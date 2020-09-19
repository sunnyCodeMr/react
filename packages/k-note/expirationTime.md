firstPendingTime
remainingExpirationTime
callbackExpirationTime
finishedExpirationTime
renderExpirationTime //记录render阶段开始时的expirationTime
updateExpirationTime //执行beginWork时记录的expirationTime


// Don't change these two values. They're used by React Dev Tools.
export const NoEffect = /*              */ 0b0000000000000; 表示没有更新
export const PerformedWork = /*         */ 0b0000000000001; 这个是开发调试会用到的

// You can change the rest (and add more).
export const Placement = /*             */ 0b0000000000010; 表示是新增的
export const Update = /*                */ 0b0000000000100; 表示节点有更新
export const PlacementAndUpdate = /*    */ 0b0000000000110; 表示节点被移动了
export const Deletion = /*              */ 0b0000000001000; 表示节点被删除了
export const ContentReset = /*          */ 0b0000000010000;
export const Callback = /*              */ 0b0000000100000; 表示类组件的setState有callback
export const DidCapture = /*            */ 0b0000001000000;
export const Ref = /*                   */ 0b0000010000000;
export const Snapshot = /*              */ 0b0000100000000;
export const Passive = /*               */ 0b0001000000000;
export const Hydrating = /*             */ 0b0010000000000;
export const HydratingAndUpdate = /*    */ 0b0010000000100;