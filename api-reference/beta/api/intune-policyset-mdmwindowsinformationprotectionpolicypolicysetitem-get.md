---
title: Obter mdmWindowsInformationProtectionPolicyPolicySetItem
description: Leia as propriedades e as relações do objeto mdmWindowsInformationProtectionPolicyPolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a476f5c1ec3c739b07dfa924ba1c16be9beaf1c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802199"
---
# <a name="get-mdmwindowsinformationprotectionpolicypolicysetitem"></a><span data-ttu-id="cb729-103">Obter mdmWindowsInformationProtectionPolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="cb729-103">Get mdmWindowsInformationProtectionPolicyPolicySetItem</span></span>

> <span data-ttu-id="cb729-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb729-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb729-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb729-106">Leia as propriedades e as relações do objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="cb729-106">Read properties and relationships of the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb729-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb729-107">Prerequisites</span></span>
<span data-ttu-id="cb729-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb729-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb729-110">Permission type</span></span>|<span data-ttu-id="cb729-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb729-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb729-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb729-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb729-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb729-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cb729-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb729-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb729-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb729-115">Not supported.</span></span>|
|<span data-ttu-id="cb729-116">Application</span><span class="sxs-lookup"><span data-stu-id="cb729-116">Application</span></span>|<span data-ttu-id="cb729-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb729-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb729-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb729-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb729-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb729-119">Optional query parameters</span></span>
<span data-ttu-id="cb729-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb729-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb729-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb729-121">Request headers</span></span>
|<span data-ttu-id="cb729-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb729-122">Header</span></span>|<span data-ttu-id="cb729-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cb729-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb729-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb729-124">Authorization</span></span>|<span data-ttu-id="cb729-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb729-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb729-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb729-126">Accept</span></span>|<span data-ttu-id="cb729-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cb729-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb729-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb729-128">Request body</span></span>
<span data-ttu-id="cb729-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb729-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb729-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb729-130">Response</span></span>
<span data-ttu-id="cb729-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb729-131">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb729-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb729-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb729-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb729-133">Request</span></span>
<span data-ttu-id="cb729-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb729-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="cb729-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb729-135">Response</span></span>
<span data-ttu-id="cb729-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb729-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": {
    "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
    "id": "4ac5be70-be70-4ac5-70be-c54a70bec54a",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ]
  }
}
```




