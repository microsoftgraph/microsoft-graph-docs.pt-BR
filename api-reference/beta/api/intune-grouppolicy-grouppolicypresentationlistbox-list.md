---
title: Listar groupPolicyPresentationListBoxes
description: Listar Propriedades e relações dos objetos groupPolicyPresentationListBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b45f8bb00b3b17bea54730aa7a4f67c67d5083
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464684"
---
# <a name="list-grouppolicypresentationlistboxes"></a><span data-ttu-id="fbccf-103">Listar groupPolicyPresentationListBoxes</span><span class="sxs-lookup"><span data-stu-id="fbccf-103">List groupPolicyPresentationListBoxes</span></span>

<span data-ttu-id="fbccf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fbccf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbccf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbccf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbccf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbccf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbccf-107">Listar Propriedades e relações dos objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="fbccf-107">List properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbccf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbccf-108">Prerequisites</span></span>
<span data-ttu-id="fbccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbccf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbccf-111">Permission type</span></span>|<span data-ttu-id="fbccf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbccf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbccf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbccf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fbccf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbccf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbccf-116">Not supported.</span></span>|
|<span data-ttu-id="fbccf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbccf-117">Application</span></span>|<span data-ttu-id="fbccf-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbccf-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbccf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="fbccf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbccf-120">Request headers</span></span>
|<span data-ttu-id="fbccf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbccf-121">Header</span></span>|<span data-ttu-id="fbccf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbccf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbccf-123">Authorization</span></span>|<span data-ttu-id="fbccf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbccf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbccf-125">Accept</span></span>|<span data-ttu-id="fbccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbccf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbccf-127">Request body</span></span>
<span data-ttu-id="fbccf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbccf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbccf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbccf-129">Response</span></span>
<span data-ttu-id="fbccf-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbccf-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbccf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbccf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbccf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbccf-132">Request</span></span>
<span data-ttu-id="fbccf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbccf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="fbccf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbccf-134">Response</span></span>
<span data-ttu-id="fbccf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbccf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 335

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
      "label": "Label value",
      "id": "2e074c87-4c87-2e07-874c-072e874c072e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "explicitValue": true,
      "valuePrefix": "Value Prefix value"
    }
  ]
}
```





