---
title: Listar groupPolicyPresentationListBoxes
description: Listar Propriedades e relações dos objetos groupPolicyPresentationListBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7eff79f2cc95be6da48fbced735a0afa250ff7cf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964665"
---
# <a name="list-grouppolicypresentationlistboxes"></a><span data-ttu-id="21bb8-103">Listar groupPolicyPresentationListBoxes</span><span class="sxs-lookup"><span data-stu-id="21bb8-103">List groupPolicyPresentationListBoxes</span></span>

> <span data-ttu-id="21bb8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21bb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bb8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21bb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bb8-106">Listar Propriedades e relações dos objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="21bb8-106">List properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21bb8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21bb8-107">Prerequisites</span></span>
<span data-ttu-id="21bb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21bb8-110">Permission type</span></span>|<span data-ttu-id="21bb8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21bb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21bb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21bb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21bb8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bb8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21bb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21bb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21bb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21bb8-115">Not supported.</span></span>|
|<span data-ttu-id="21bb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21bb8-116">Application</span></span>|<span data-ttu-id="21bb8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21bb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21bb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21bb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="21bb8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21bb8-119">Request headers</span></span>
|<span data-ttu-id="21bb8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21bb8-120">Header</span></span>|<span data-ttu-id="21bb8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21bb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21bb8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21bb8-122">Authorization</span></span>|<span data-ttu-id="21bb8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21bb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21bb8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21bb8-124">Accept</span></span>|<span data-ttu-id="21bb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21bb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21bb8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21bb8-126">Request body</span></span>
<span data-ttu-id="21bb8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21bb8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21bb8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bb8-128">Response</span></span>
<span data-ttu-id="21bb8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21bb8-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bb8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21bb8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="21bb8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21bb8-131">Request</span></span>
<span data-ttu-id="21bb8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21bb8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="21bb8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bb8-133">Response</span></span>
<span data-ttu-id="21bb8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21bb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
      "label": "Label value",
      "id": "2e074c87-4c87-2e07-874c-072e874c072e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "explicitValue": true
    }
  ]
}
```





