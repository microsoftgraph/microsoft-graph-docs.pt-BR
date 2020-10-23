---
title: Obter groupPolicyUploadedCategory
description: Leia as propriedades e as relações do objeto groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 251e00c09e75e70644e6dc9e66df7f1f8ba275ff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695520"
---
# <a name="get-grouppolicyuploadedcategory"></a><span data-ttu-id="b687c-103">Obter groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="b687c-103">Get groupPolicyUploadedCategory</span></span>

<span data-ttu-id="b687c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b687c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b687c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b687c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b687c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b687c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b687c-107">Leia as propriedades e as relações do objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="b687c-107">Read properties and relationships of the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b687c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b687c-108">Prerequisites</span></span>
<span data-ttu-id="b687c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b687c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b687c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b687c-111">Permission type</span></span>|<span data-ttu-id="b687c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b687c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b687c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b687c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b687c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b687c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b687c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b687c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b687c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b687c-116">Not supported.</span></span>|
|<span data-ttu-id="b687c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b687c-117">Application</span></span>|<span data-ttu-id="b687c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b687c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b687c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b687c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/parent
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children/{groupPolicyCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b687c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b687c-120">Optional query parameters</span></span>
<span data-ttu-id="b687c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b687c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b687c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b687c-122">Request headers</span></span>
|<span data-ttu-id="b687c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b687c-123">Header</span></span>|<span data-ttu-id="b687c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b687c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b687c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b687c-125">Authorization</span></span>|<span data-ttu-id="b687c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b687c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b687c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b687c-127">Accept</span></span>|<span data-ttu-id="b687c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b687c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b687c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b687c-129">Request body</span></span>
<span data-ttu-id="b687c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b687c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b687c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b687c-131">Response</span></span>
<span data-ttu-id="b687c-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b687c-132">If successful, this method returns a `200 OK` response code and [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b687c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b687c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b687c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b687c-134">Request</span></span>
<span data-ttu-id="b687c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b687c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
```

### <a name="response"></a><span data-ttu-id="b687c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b687c-136">Response</span></span>
<span data-ttu-id="b687c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b687c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
    "displayName": "Display Name value",
    "isRoot": true,
    "id": "7e373e80-3e80-7e37-803e-377e803e377e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





