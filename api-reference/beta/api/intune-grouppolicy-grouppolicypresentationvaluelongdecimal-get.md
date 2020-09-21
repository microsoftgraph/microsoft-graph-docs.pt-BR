---
title: Obter groupPolicyPresentationValueLongDecimal
description: Leia as propriedades e as relações do objeto groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39c595c13fce5bcc37b4877f4f606143d4ab9445
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000515"
---
# <a name="get-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="2e952-103">Obter groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="2e952-103">Get groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="2e952-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e952-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e952-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e952-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e952-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e952-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e952-107">Leia as propriedades e as relações do objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2e952-107">Read properties and relationships of the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e952-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e952-108">Prerequisites</span></span>
<span data-ttu-id="2e952-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e952-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e952-111">Permission type</span></span>|<span data-ttu-id="2e952-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e952-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e952-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e952-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e952-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e952-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e952-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e952-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e952-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e952-116">Not supported.</span></span>|
|<span data-ttu-id="2e952-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e952-117">Application</span></span>|<span data-ttu-id="2e952-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e952-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e952-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e952-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e952-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e952-120">Optional query parameters</span></span>
<span data-ttu-id="2e952-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e952-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e952-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e952-122">Request headers</span></span>
|<span data-ttu-id="2e952-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e952-123">Header</span></span>|<span data-ttu-id="2e952-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2e952-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e952-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e952-125">Authorization</span></span>|<span data-ttu-id="2e952-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e952-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e952-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e952-127">Accept</span></span>|<span data-ttu-id="2e952-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e952-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e952-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e952-129">Request body</span></span>
<span data-ttu-id="2e952-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e952-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e952-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e952-131">Response</span></span>
<span data-ttu-id="2e952-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e952-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e952-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e952-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e952-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e952-134">Request</span></span>
<span data-ttu-id="2e952-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e952-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="2e952-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e952-136">Response</span></span>
<span data-ttu-id="2e952-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e952-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "210f7078-7078-210f-7870-0f2178700f21",
    "value": 5
  }
}
```






