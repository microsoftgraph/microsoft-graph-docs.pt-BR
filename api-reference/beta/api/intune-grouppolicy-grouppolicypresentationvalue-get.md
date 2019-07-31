---
title: Obter groupPolicyPresentationValue
description: Leia as propriedades e as relações do objeto groupPolicyPresentationValue.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81afb3c1643fe282a2b7bb26057b7aec3bcf1e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989312"
---
# <a name="get-grouppolicypresentationvalue"></a><span data-ttu-id="91b34-103">Obter groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="91b34-103">Get groupPolicyPresentationValue</span></span>

> <span data-ttu-id="91b34-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91b34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91b34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91b34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91b34-106">Leia as propriedades e as relações do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="91b34-106">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91b34-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91b34-107">Prerequisites</span></span>
<span data-ttu-id="91b34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b34-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91b34-110">Permission type</span></span>|<span data-ttu-id="91b34-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91b34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91b34-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91b34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91b34-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b34-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="91b34-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91b34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91b34-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91b34-115">Not supported.</span></span>|
|<span data-ttu-id="91b34-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91b34-116">Application</span></span>|<span data-ttu-id="91b34-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91b34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91b34-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91b34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91b34-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91b34-119">Optional query parameters</span></span>
<span data-ttu-id="91b34-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91b34-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91b34-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91b34-121">Request headers</span></span>
|<span data-ttu-id="91b34-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91b34-122">Header</span></span>|<span data-ttu-id="91b34-123">Valor</span><span class="sxs-lookup"><span data-stu-id="91b34-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91b34-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="91b34-124">Authorization</span></span>|<span data-ttu-id="91b34-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b34-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91b34-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91b34-126">Accept</span></span>|<span data-ttu-id="91b34-127">application/json</span><span class="sxs-lookup"><span data-stu-id="91b34-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91b34-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91b34-128">Request body</span></span>
<span data-ttu-id="91b34-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91b34-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91b34-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b34-130">Response</span></span>
<span data-ttu-id="91b34-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b34-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91b34-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91b34-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="91b34-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91b34-133">Request</span></span>
<span data-ttu-id="91b34-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b34-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="91b34-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b34-135">Response</span></span>
<span data-ttu-id="91b34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91b34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "8132eaab-eaab-8132-abea-3281abea3281"
  }
}
```





