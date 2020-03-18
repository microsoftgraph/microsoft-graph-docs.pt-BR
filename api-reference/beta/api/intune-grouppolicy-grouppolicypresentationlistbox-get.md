---
title: Obter groupPolicyPresentationListBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationListBox.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6878f3d63c29b6e0c5405fc24460835d04c261fd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804202"
---
# <a name="get-grouppolicypresentationlistbox"></a><span data-ttu-id="34258-103">Obter groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="34258-103">Get groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="34258-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34258-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34258-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34258-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34258-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="34258-106">Read properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34258-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34258-107">Prerequisites</span></span>
<span data-ttu-id="34258-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34258-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34258-110">Permission type</span></span>|<span data-ttu-id="34258-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34258-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34258-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34258-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34258-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34258-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="34258-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34258-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34258-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34258-115">Not supported.</span></span>|
|<span data-ttu-id="34258-116">Application</span><span class="sxs-lookup"><span data-stu-id="34258-116">Application</span></span>|<span data-ttu-id="34258-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34258-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34258-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34258-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34258-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34258-119">Optional query parameters</span></span>
<span data-ttu-id="34258-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34258-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34258-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34258-121">Request headers</span></span>
|<span data-ttu-id="34258-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34258-122">Header</span></span>|<span data-ttu-id="34258-123">Valor</span><span class="sxs-lookup"><span data-stu-id="34258-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34258-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="34258-124">Authorization</span></span>|<span data-ttu-id="34258-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34258-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34258-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34258-126">Accept</span></span>|<span data-ttu-id="34258-127">application/json</span><span class="sxs-lookup"><span data-stu-id="34258-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34258-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34258-128">Request body</span></span>
<span data-ttu-id="34258-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34258-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34258-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="34258-130">Response</span></span>
<span data-ttu-id="34258-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34258-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34258-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34258-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="34258-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34258-133">Request</span></span>
<span data-ttu-id="34258-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34258-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="34258-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="34258-135">Response</span></span>
<span data-ttu-id="34258-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34258-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
    "label": "Label value",
    "id": "2e074c87-4c87-2e07-874c-072e874c072e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "explicitValue": true,
    "valuePrefix": "Value Prefix value"
  }
}
```




