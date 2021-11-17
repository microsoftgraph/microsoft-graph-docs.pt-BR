---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2907a4fb2c9b5444d380765c4dfb44e189a31207
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetQueryParameters{
    Select: "key",
}
options := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetOptions{
    Q: requestParameters,
}
bitlockerRecoveryKeyId := "bitlockerRecoveryKey-id"
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeysById(&bitlockerRecoveryKeyId).Get(options)


```