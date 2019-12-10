---
title: Listar groupPolicyPresentationTexts
description: Listar Propriedades e relações dos objetos groupPolicyPresentationText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c5b6b9031aaa29bebb2cb4d6428a51073e59c63
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942805"
---
# <a name="list-grouppolicypresentationtexts"></a><span data-ttu-id="c2788-103">Listar groupPolicyPresentationTexts</span><span class="sxs-lookup"><span data-stu-id="c2788-103">List groupPolicyPresentationTexts</span></span>

> <span data-ttu-id="c2788-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2788-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2788-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="c2788-106">List properties and relationships of the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2788-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2788-107">Prerequisites</span></span>
<span data-ttu-id="c2788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2788-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2788-110">Permission type</span></span>|<span data-ttu-id="c2788-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2788-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2788-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2788-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c2788-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2788-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2788-115">Not supported.</span></span>|
|<span data-ttu-id="c2788-116">Application</span><span class="sxs-lookup"><span data-stu-id="c2788-116">Application</span></span>|<span data-ttu-id="c2788-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2788-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2788-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="c2788-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2788-119">Request headers</span></span>
|<span data-ttu-id="c2788-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2788-120">Header</span></span>|<span data-ttu-id="c2788-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c2788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2788-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2788-122">Authorization</span></span>|<span data-ttu-id="c2788-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2788-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2788-124">Accept</span></span>|<span data-ttu-id="c2788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2788-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2788-126">Request body</span></span>
<span data-ttu-id="c2788-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2788-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2788-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2788-128">Response</span></span>
<span data-ttu-id="c2788-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2788-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2788-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2788-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2788-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2788-131">Request</span></span>
<span data-ttu-id="c2788-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2788-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="c2788-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2788-133">Response</span></span>
<span data-ttu-id="c2788-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2788-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





