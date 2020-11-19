---
title: Listar groupPolicyObjectFiles
description: Listar Propriedades e relações dos objetos groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc125eeea595c97bc0b45c1423b1ba702293bda1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277992"
---
# <a name="list-grouppolicyobjectfiles"></a><span data-ttu-id="94a6b-103">Listar groupPolicyObjectFiles</span><span class="sxs-lookup"><span data-stu-id="94a6b-103">List groupPolicyObjectFiles</span></span>

<span data-ttu-id="94a6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94a6b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94a6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94a6b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94a6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94a6b-107">Listar Propriedades e relações dos objetos [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="94a6b-107">List properties and relationships of the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94a6b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94a6b-108">Prerequisites</span></span>
<span data-ttu-id="94a6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a6b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a6b-111">Permission type</span></span>|<span data-ttu-id="94a6b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94a6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94a6b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94a6b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94a6b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94a6b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94a6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a6b-116">Not supported.</span></span>|
|<span data-ttu-id="94a6b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a6b-117">Application</span></span>|<span data-ttu-id="94a6b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94a6b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94a6b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="94a6b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a6b-120">Request headers</span></span>
|<span data-ttu-id="94a6b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94a6b-121">Header</span></span>|<span data-ttu-id="94a6b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="94a6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94a6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a6b-123">Authorization</span></span>|<span data-ttu-id="94a6b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94a6b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94a6b-125">Accept</span></span>|<span data-ttu-id="94a6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94a6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a6b-127">Request body</span></span>
<span data-ttu-id="94a6b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94a6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a6b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a6b-129">Response</span></span>
<span data-ttu-id="94a6b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a6b-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a6b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a6b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="94a6b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a6b-132">Request</span></span>
<span data-ttu-id="94a6b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a6b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
```

### <a name="response"></a><span data-ttu-id="94a6b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a6b-134">Response</span></span>
<span data-ttu-id="94a6b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94a6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
      "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
      "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "content": "Content value"
    }
  ]
}
```




