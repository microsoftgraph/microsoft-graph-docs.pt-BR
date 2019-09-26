---
title: Listar groupPolicyPresentationTexts
description: Listar Propriedades e relações dos objetos groupPolicyPresentationText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03ef4c7e8a7ff9df5d7723882e342a6b1a071f99
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194051"
---
# <a name="list-grouppolicypresentationtexts"></a><span data-ttu-id="bb87c-103">Listar groupPolicyPresentationTexts</span><span class="sxs-lookup"><span data-stu-id="bb87c-103">List groupPolicyPresentationTexts</span></span>

> <span data-ttu-id="bb87c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb87c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb87c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb87c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb87c-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="bb87c-106">List properties and relationships of the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb87c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb87c-107">Prerequisites</span></span>
<span data-ttu-id="bb87c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb87c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb87c-110">Permission type</span></span>|<span data-ttu-id="bb87c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb87c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb87c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb87c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb87c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb87c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="bb87c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb87c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb87c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb87c-115">Not supported.</span></span>|
|<span data-ttu-id="bb87c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb87c-116">Application</span></span>|<span data-ttu-id="bb87c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb87c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb87c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb87c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="bb87c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb87c-119">Request headers</span></span>
|<span data-ttu-id="bb87c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb87c-120">Header</span></span>|<span data-ttu-id="bb87c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb87c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb87c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb87c-122">Authorization</span></span>|<span data-ttu-id="bb87c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb87c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb87c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb87c-124">Accept</span></span>|<span data-ttu-id="bb87c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb87c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb87c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb87c-126">Request body</span></span>
<span data-ttu-id="bb87c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb87c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb87c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb87c-128">Response</span></span>
<span data-ttu-id="bb87c-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb87c-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb87c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb87c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb87c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb87c-131">Request</span></span>
<span data-ttu-id="bb87c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb87c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="bb87c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb87c-133">Response</span></span>
<span data-ttu-id="bb87c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb87c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 258

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
      "label": "Label value",
      "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




