[@wholebuzz/fs](../README.md) / [Exports](../modules.md) / [fs](../modules/fs.md) / AnyFileSystem

# Class: AnyFileSystem

[fs](../modules/fs.md).AnyFileSystem

Class Adapter Pattern wrapping [FileSystem](fs.filesystem.md) by `urlPrefix`.

## Hierarchy

- [*FileSystem*](fs.filesystem.md)

  ↳ **AnyFileSystem**

## Table of contents

### Constructors

- [constructor](fs.anyfilesystem.md#constructor)

### Properties

- [supported](fs.anyfilesystem.md#supported)

### Methods

- [appendToFile](fs.anyfilesystem.md#appendtofile)
- [copyFile](fs.anyfilesystem.md#copyfile)
- [createFile](fs.anyfilesystem.md#createfile)
- [ensureDirectory](fs.anyfilesystem.md#ensuredirectory)
- [fileExists](fs.anyfilesystem.md#fileexists)
- [getFileStatus](fs.anyfilesystem.md#getfilestatus)
- [getFs](fs.anyfilesystem.md#getfs)
- [moveFile](fs.anyfilesystem.md#movefile)
- [openReadableFile](fs.anyfilesystem.md#openreadablefile)
- [openWritableFile](fs.anyfilesystem.md#openwritablefile)
- [queueRemoveFile](fs.anyfilesystem.md#queueremovefile)
- [readDirectory](fs.anyfilesystem.md#readdirectory)
- [readDirectoryStream](fs.anyfilesystem.md#readdirectorystream)
- [removeDirectory](fs.anyfilesystem.md#removedirectory)
- [removeFile](fs.anyfilesystem.md#removefile)
- [replaceFile](fs.anyfilesystem.md#replacefile)

## Constructors

### constructor

\+ **new AnyFileSystem**(`supported`: { `fs`: [*FileSystem*](fs.filesystem.md) ; `urlPrefix`: *string*  }[]): [*AnyFileSystem*](fs.anyfilesystem.md)

Construct an [AnyFileSystem](fs.anyfilesystem.md) wrapping the provided [FileSystem](fs.filesystem.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `supported` | { `fs`: [*FileSystem*](fs.filesystem.md) ; `urlPrefix`: *string*  }[] | The [FileSystem](fs.filesystem.md) to delegate according to `urlPrefix`. |

**Returns:** [*AnyFileSystem*](fs.anyfilesystem.md)

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:215](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L215)

## Properties

### supported

• **supported**: { `fs`: [*FileSystem*](fs.filesystem.md) ; `urlPrefix`: *string*  }[]

## Methods

### appendToFile

▸ **appendToFile**(`urlText`: *string*, `writeCallback`: (`stream`: WritableStreamTree) => *Promise*<boolean\>, `createCallback?`: (`stream`: WritableStreamTree) => *Promise*<boolean\>, `createOptions?`: [*CreateOptions*](../interfaces/fs.createoptions.md), `appendOptions?`: [*AppendOptions*](../interfaces/fs.appendoptions.md)): *Promise*<``null`` \| [*FileStatus*](../interfaces/fs.filestatus.md)\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `writeCallback` | (`stream`: WritableStreamTree) => *Promise*<boolean\> |
| `createCallback?` | (`stream`: WritableStreamTree) => *Promise*<boolean\> |
| `createOptions?` | [*CreateOptions*](../interfaces/fs.createoptions.md) |
| `appendOptions?` | [*AppendOptions*](../interfaces/fs.appendoptions.md) |

**Returns:** *Promise*<``null`` \| [*FileStatus*](../interfaces/fs.filestatus.md)\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:312](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L312)

___

### copyFile

▸ **copyFile**(`sourceUrlText`: *string*, `destUrlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `sourceUrlText` | *string* |
| `destUrlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:293](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L293)

___

### createFile

▸ **createFile**(`urlText`: *string*, `createCallback?`: (`stream`: WritableStreamTree) => *Promise*<boolean\>, `options?`: [*CreateOptions*](../interfaces/fs.createoptions.md)): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `createCallback?` | (`stream`: WritableStreamTree) => *Promise*<boolean\> |
| `options?` | [*CreateOptions*](../interfaces/fs.createoptions.md) |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:274](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L274)

___

### ensureDirectory

▸ **ensureDirectory**(`urlText`: *string*, `options?`: [*EnsureDirectoryOptions*](../interfaces/fs.ensuredirectoryoptions.md)): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `options?` | [*EnsureDirectoryOptions*](../interfaces/fs.ensuredirectoryoptions.md) |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:244](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L244)

___

### fileExists

▸ **fileExists**(`urlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:254](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L254)

___

### getFileStatus

▸ **getFileStatus**(`urlText`: *string*, `options?`: [*GetFileStatusOptions*](../interfaces/fs.getfilestatusoptions.md)): *Promise*<[*FileStatus*](../interfaces/fs.filestatus.md)\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `options?` | [*GetFileStatusOptions*](../interfaces/fs.getfilestatusoptions.md) |

**Returns:** *Promise*<[*FileStatus*](../interfaces/fs.filestatus.md)\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:259](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L259)

___

### getFs

▸ **getFs**(`url`: *string*): [*FileSystem*](fs.filesystem.md)

Returns the [FileSystem](fs.filesystem.md) provider for `url`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | *string* | The URL of the file. |

**Returns:** [*FileSystem*](fs.filesystem.md)

Defined in: [src/fs.ts:228](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L228)

___

### moveFile

▸ **moveFile**(`sourceUrlText`: *string*, `destUrlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `sourceUrlText` | *string* |
| `destUrlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:298](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L298)

___

### openReadableFile

▸ **openReadableFile**(`url`: *string*, `options?`: [*OpenReadableFileOptions*](../interfaces/fs.openreadablefileoptions.md)): *Promise*<ReadableStreamTree\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | *string* |
| `options?` | [*OpenReadableFileOptions*](../interfaces/fs.openreadablefileoptions.md) |

**Returns:** *Promise*<ReadableStreamTree\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:264](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L264)

___

### openWritableFile

▸ **openWritableFile**(`url`: *string*, `options?`: [*OpenWritableFileOptions*](../interfaces/fs.openwritablefileoptions.md)): *Promise*<WritableStreamTree\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | *string* |
| `options?` | [*OpenWritableFileOptions*](../interfaces/fs.openwritablefileoptions.md) |

**Returns:** *Promise*<WritableStreamTree\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:269](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L269)

___

### queueRemoveFile

▸ **queueRemoveFile**(`urlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:288](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L288)

___

### readDirectory

▸ **readDirectory**(`urlText`: *string*, `options?`: [*ReadDirectoryOptions*](../interfaces/fs.readdirectoryoptions.md)): *Promise*<[*DirectoryEntry*](../interfaces/fs.directoryentry.md)[]\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `options?` | [*ReadDirectoryOptions*](../interfaces/fs.readdirectoryoptions.md) |

**Returns:** *Promise*<[*DirectoryEntry*](../interfaces/fs.directoryentry.md)[]\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:234](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L234)

___

### readDirectoryStream

▸ **readDirectoryStream**(`urlText`: *string*, `options?`: [*ReadDirectoryOptions*](../interfaces/fs.readdirectoryoptions.md)): *Promise*<ReadableStreamTree\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `options?` | [*ReadDirectoryOptions*](../interfaces/fs.readdirectoryoptions.md) |

**Returns:** *Promise*<ReadableStreamTree\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:239](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L239)

___

### removeDirectory

▸ **removeDirectory**(`urlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:249](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L249)

___

### removeFile

▸ **removeFile**(`urlText`: *string*): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:283](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L283)

___

### replaceFile

▸ **replaceFile**(`urlText`: *string*, `writeCallback`: (`stream`: WritableStreamTree) => *Promise*<boolean\>, `options?`: [*ReplaceFileOptions*](../interfaces/fs.replacefileoptions.md)): *Promise*<boolean\>

**`inheritdoc`**

#### Parameters

| Name | Type |
| :------ | :------ |
| `urlText` | *string* |
| `writeCallback` | (`stream`: WritableStreamTree) => *Promise*<boolean\> |
| `options?` | [*ReplaceFileOptions*](../interfaces/fs.replacefileoptions.md) |

**Returns:** *Promise*<boolean\>

Overrides: [FileSystem](fs.filesystem.md)

Defined in: [src/fs.ts:303](https://github.com/wholebuzz/fs/blob/master/src/fs.ts#L303)
