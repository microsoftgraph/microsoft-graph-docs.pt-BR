---
title: Listar mdmWindowsInformationProtectionPolicyPolicySetItems
description: Listar propriedades e relações dos objetos mdmWindowsInformationProtectionPolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74c487b4339995694858170cc50f7b470f12c29f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158609"
---
# <a name="list-mdmwindowsinformationprotectionpolicypolicysetitems"></a><span data-ttu-id="285e2-103">Listar mdmWindowsInformationProtectionPolicyPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="285e2-103">List mdmWindowsInformationProtectionPolicyPolicySetItems</span></span>

<span data-ttu-id="285e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="285e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="285e2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="285e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="285e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="285e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="285e2-107">Listar propriedades e relações dos [objetos mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="285e2-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="285e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="285e2-108">Prerequisites</span></span>
<span data-ttu-id="285e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="285e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="285e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="285e2-111">Permission type</span></span>|<span data-ttu-id="285e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="285e2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="285e2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="285e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="285e2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285e2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="285e2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="285e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="285e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="285e2-116">Not supported.</span></span>|
|<span data-ttu-id="285e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="285e2-117">Application</span></span>|<span data-ttu-id="285e2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285e2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="285e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="285e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="285e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="285e2-120">Request headers</span></span>
|<span data-ttu-id="285e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="285e2-121">Header</span></span>|<span data-ttu-id="285e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="285e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="285e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="285e2-123">Authorization</span></span>|<span data-ttu-id="285e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="285e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="285e2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="285e2-125">Accept</span></span>|<span data-ttu-id="285e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="285e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="285e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="285e2-127">Request body</span></span>
<span data-ttu-id="285e2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="285e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="285e2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="285e2-129">Response</span></span>
<span data-ttu-id="285e2-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="285e2-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="285e2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="285e2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="285e2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="285e2-132">Request</span></span>
<span data-ttu-id="285e2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="285e2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="285e2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="285e2-134">Response</span></span>
<span data-ttu-id="285e2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="285e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
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
  ]
}
```




