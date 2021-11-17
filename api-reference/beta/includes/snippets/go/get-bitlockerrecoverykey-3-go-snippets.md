---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 548d3943cd1aa8bf363495b6f7a1bde7cbf27f2d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "ocp-client-name": ""My Friendly Client""
    "ocp-client-version": ""1.2""
}
options := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetOptions{
    H: headers,
}
bitlockerRecoveryKeyId := "bitlockerRecoveryKey-id"
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeysById(&bitlockerRecoveryKeyId).Get(options)


```