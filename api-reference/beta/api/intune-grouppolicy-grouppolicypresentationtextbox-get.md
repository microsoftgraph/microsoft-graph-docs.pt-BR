---
title: Obter groupPolicyPresentationTextBox
description: Leia as propriedades e as relações do objeto groupPolicyPresentationTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef3351ac0d5b5f860b93d0eb1c456333c928dfd7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151713"
---
# <a name="get-grouppolicypresentationtextbox"></a><span data-ttu-id="6e011-103">Obter groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="6e011-103">Get groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="6e011-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e011-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e011-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e011-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e011-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="6e011-106">Read properties and relationships of the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e011-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e011-107">Prerequisites</span></span>
<span data-ttu-id="6e011-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e011-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e011-110">Permission type</span></span>|<span data-ttu-id="6e011-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e011-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e011-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e011-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e011-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e011-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6e011-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e011-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e011-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e011-115">Not supported.</span></span>|
|<span data-ttu-id="6e011-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e011-116">Application</span></span>|<span data-ttu-id="6e011-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e011-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e011-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e011-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e011-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e011-119">Optional query parameters</span></span>
<span data-ttu-id="6e011-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e011-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e011-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e011-121">Request headers</span></span>
|<span data-ttu-id="6e011-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e011-122">Header</span></span>|<span data-ttu-id="6e011-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6e011-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e011-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e011-124">Authorization</span></span>|<span data-ttu-id="6e011-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e011-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e011-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e011-126">Accept</span></span>|<span data-ttu-id="6e011-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6e011-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e011-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e011-128">Request body</span></span>
<span data-ttu-id="6e011-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e011-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e011-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e011-130">Response</span></span>
<span data-ttu-id="6e011-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e011-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e011-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e011-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e011-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e011-133">Request</span></span>
<span data-ttu-id="6e011-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e011-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="6e011-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e011-135">Response</span></span>
<span data-ttu-id="6e011-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e011-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
    "label": "Label value",
    "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "required": true,
    "maxLength": 9
  }
}
```




