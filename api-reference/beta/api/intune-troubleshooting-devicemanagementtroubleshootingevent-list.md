---
title: Listar deviceManagementTroubleshootingEvents
description: Listar propriedades e relações de objetos de deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7b5e63228dd36d8f44f058829fe01586f127f89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134106"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="dedab-103">Listar deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="dedab-103">List deviceManagementTroubleshootingEvents</span></span>

<span data-ttu-id="dedab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dedab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dedab-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dedab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dedab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dedab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dedab-107">Listar propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="dedab-107">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dedab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dedab-108">Prerequisites</span></span>
<span data-ttu-id="dedab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dedab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dedab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dedab-111">Permission type</span></span>|<span data-ttu-id="dedab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dedab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dedab-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dedab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dedab-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dedab-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dedab-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dedab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dedab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dedab-116">Not supported.</span></span>|
|<span data-ttu-id="dedab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dedab-117">Application</span></span>|<span data-ttu-id="dedab-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dedab-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dedab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dedab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="dedab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dedab-120">Request headers</span></span>
|<span data-ttu-id="dedab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dedab-121">Header</span></span>|<span data-ttu-id="dedab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dedab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dedab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dedab-123">Authorization</span></span>|<span data-ttu-id="dedab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dedab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dedab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dedab-125">Accept</span></span>|<span data-ttu-id="dedab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dedab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dedab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dedab-127">Request body</span></span>
<span data-ttu-id="dedab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dedab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dedab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dedab-129">Response</span></span>
<span data-ttu-id="dedab-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dedab-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dedab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dedab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dedab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dedab-132">Request</span></span>
<span data-ttu-id="dedab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dedab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="dedab-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dedab-134">Response</span></span>
<span data-ttu-id="dedab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dedab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```




