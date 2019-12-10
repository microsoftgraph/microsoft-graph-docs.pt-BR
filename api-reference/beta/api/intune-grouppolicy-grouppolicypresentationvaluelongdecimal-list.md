---
title: Listar groupPolicyPresentationValueLongDecimals
description: Listar Propriedades e relações dos objetos groupPolicyPresentationValueLongDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf491da0a3b90bf45891c4fb964cc412691cb3dc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942700"
---
# <a name="list-grouppolicypresentationvaluelongdecimals"></a><span data-ttu-id="4c780-103">Listar groupPolicyPresentationValueLongDecimals</span><span class="sxs-lookup"><span data-stu-id="4c780-103">List groupPolicyPresentationValueLongDecimals</span></span>

> <span data-ttu-id="4c780-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c780-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c780-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c780-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="4c780-106">List properties and relationships of the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c780-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c780-107">Prerequisites</span></span>
<span data-ttu-id="4c780-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c780-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c780-110">Permission type</span></span>|<span data-ttu-id="4c780-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c780-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c780-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c780-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c780-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c780-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4c780-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c780-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c780-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c780-115">Not supported.</span></span>|
|<span data-ttu-id="4c780-116">Application</span><span class="sxs-lookup"><span data-stu-id="4c780-116">Application</span></span>|<span data-ttu-id="4c780-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c780-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c780-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c780-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="4c780-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c780-119">Request headers</span></span>
|<span data-ttu-id="4c780-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c780-120">Header</span></span>|<span data-ttu-id="4c780-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c780-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c780-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c780-122">Authorization</span></span>|<span data-ttu-id="4c780-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c780-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c780-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c780-124">Accept</span></span>|<span data-ttu-id="4c780-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c780-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c780-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c780-126">Request body</span></span>
<span data-ttu-id="4c780-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c780-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c780-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c780-128">Response</span></span>
<span data-ttu-id="4c780-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c780-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c780-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c780-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c780-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c780-131">Request</span></span>
<span data-ttu-id="4c780-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c780-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="4c780-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c780-133">Response</span></span>
<span data-ttu-id="4c780-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c780-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "210f7078-7078-210f-7870-0f2178700f21",
      "value": 5
    }
  ]
}
```





