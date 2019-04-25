---
title: Obter groupPolicyPresentationComboBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationComboBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1c7010a75ea31c9fb238845a1c562786638831
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531177"
---
# <a name="get-grouppolicypresentationcombobox"></a><span data-ttu-id="c7eab-103">Obter groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="c7eab-103">Get groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="c7eab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7eab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7eab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7eab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7eab-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="c7eab-106">Read properties and relationships of the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7eab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7eab-107">Prerequisites</span></span>
<span data-ttu-id="c7eab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7eab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7eab-110">Permission type</span></span>|<span data-ttu-id="c7eab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7eab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7eab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7eab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7eab-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7eab-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c7eab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7eab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7eab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7eab-115">Not supported.</span></span>|
|<span data-ttu-id="c7eab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7eab-116">Application</span></span>|<span data-ttu-id="c7eab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7eab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7eab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7eab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7eab-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7eab-119">Optional query parameters</span></span>
<span data-ttu-id="c7eab-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7eab-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7eab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7eab-121">Request headers</span></span>
|<span data-ttu-id="c7eab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7eab-122">Header</span></span>|<span data-ttu-id="c7eab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c7eab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7eab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7eab-124">Authorization</span></span>|<span data-ttu-id="c7eab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7eab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7eab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7eab-126">Accept</span></span>|<span data-ttu-id="c7eab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7eab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7eab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7eab-128">Request body</span></span>
<span data-ttu-id="c7eab-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7eab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7eab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7eab-130">Response</span></span>
<span data-ttu-id="c7eab-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7eab-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7eab-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7eab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7eab-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7eab-133">Request</span></span>
<span data-ttu-id="c7eab-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7eab-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="c7eab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7eab-135">Response</span></span>
<span data-ttu-id="c7eab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7eab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
    "label": "Label value",
    "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "suggestions": [
      "Suggestions value"
    ],
    "required": true,
    "maxLength": 9
  }
}
```





