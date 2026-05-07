# Joker Bear

`Joker Bear` 是一个给 Codex 使用的原创数字宠物素材包。

它的风格是一只白色、线条简洁、带一点自嘲气质的小熊。这个包里只保留了角色本体和它的动作精灵图，适合直接接到宠物展示界面里使用。

## 包内容

- `pet.json`：宠物基本信息与精灵图入口。
- `spritesheet.webp`：角色动作精灵图。

## 动作说明

这个角色在当前实现里的动作表现是：

- `run`：拖动时使用，也会在思考过程中显示。
- `fantasy`：思考完成后显示。
- `idle`：静止待机时使用。

## 基本信息

- `id`: `jokebear`
- `displayName`: `Joke Bear`
- `description`: `An original self-mocking white bear digital pet for Codex.`

## 使用方式

在外层应用中读取 `pet.json`，再加载 `spritesheet.webp` 即可。具体动作切换不在这个包里控制，而是由展示层根据当前状态决定。

## 备注

如果你之后还想调整表现，建议把“拖动中”和“思考中”分成不同状态，这样 `run` 和 `fantasy` 的切换会更清楚。
