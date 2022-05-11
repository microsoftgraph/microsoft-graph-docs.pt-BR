---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bb14602f3225092095de1c579aabfd4be49d5f0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "Test Printer"
requestBody.SetDisplayName(&displayName)
manufacturer := "Test Printer Manufacturer"
requestBody.SetManufacturer(&manufacturer)
model := "Test Printer Model"
requestBody.SetModel(&model)
requestBody.SetPhysicalDeviceId(nil)
hasPhysicalDevice := false
requestBody.SetHasPhysicalDevice(&hasPhysicalDevice)
certificateSigningRequest := msgraphsdk.NewPrintCertificateSigningRequest()
requestBody.SetCertificateSigningRequest(certificateSigningRequest)
content := "{content}"
certificateSigningRequest.SetContent(&content)
transportKey := "{sampleTransportKey}"
certificateSigningRequest.SetTransportKey(&transportKey)
requestBody.SetConnectorId(nil)
graphClient.Print().Printers().Create().Post(requestBody)


```