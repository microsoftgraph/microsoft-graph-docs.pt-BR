---
title: Listar groupPolicyUploadedCategories
description: Listar Propriedades e relações dos objetos groupPolicyUploadedCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09a136ae6891f31ae67907ed38022a92e84784b2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803775"
---
# <a name="list-grouppolicyuploadedcategories"></a><span data-ttu-id="46565-103">Listar groupPolicyUploadedCategories</span><span class="sxs-lookup"><span data-stu-id="46565-103">List groupPolicyUploadedCategories</span></span>

> <span data-ttu-id="46565-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46565-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46565-106">Listar Propriedades e relações dos objetos [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="46565-106">List properties and relationships of the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46565-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46565-107">Prerequisites</span></span>
<span data-ttu-id="46565-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46565-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46565-110">Permission type</span></span>|<span data-ttu-id="46565-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46565-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46565-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46565-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46565-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46565-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="46565-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46565-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46565-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46565-115">Not supported.</span></span>|
|<span data-ttu-id="46565-116">Application</span><span class="sxs-lookup"><span data-stu-id="46565-116">Application</span></span>|<span data-ttu-id="46565-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46565-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46565-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyCategories
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="46565-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46565-119">Request headers</span></span>
|<span data-ttu-id="46565-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46565-120">Header</span></span>|<span data-ttu-id="46565-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46565-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46565-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46565-122">Authorization</span></span>|<span data-ttu-id="46565-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46565-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46565-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46565-124">Accept</span></span>|<span data-ttu-id="46565-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46565-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46565-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46565-126">Request body</span></span>
<span data-ttu-id="46565-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46565-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46565-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46565-128">Response</span></span>
<span data-ttu-id="46565-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46565-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46565-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46565-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46565-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46565-131">Request</span></span>
<span data-ttu-id="46565-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46565-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
```

### <a name="response"></a><span data-ttu-id="46565-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46565-133">Response</span></span>
<span data-ttu-id="46565-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46565-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
      "displayName": "Display Name value",
      "isRoot": true,
      "id": "7e373e80-3e80-7e37-803e-377e803e377e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




