---
title: Listar groupPolicyPresentationDropdownLists
description: Listar Propriedades e relações dos objetos groupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e52b12fc829f4fbced89efe8a36741e4fcfe0460
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724681"
---
# <a name="list-grouppolicypresentationdropdownlists"></a><span data-ttu-id="eed79-103">Listar groupPolicyPresentationDropdownLists</span><span class="sxs-lookup"><span data-stu-id="eed79-103">List groupPolicyPresentationDropdownLists</span></span>

<span data-ttu-id="eed79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eed79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eed79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eed79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eed79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eed79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed79-107">Listar Propriedades e relações dos objetos [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="eed79-107">List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eed79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eed79-108">Prerequisites</span></span>
<span data-ttu-id="eed79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed79-111">Permission type</span></span>|<span data-ttu-id="eed79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eed79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eed79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eed79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eed79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eed79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eed79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed79-116">Not supported.</span></span>|
|<span data-ttu-id="eed79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eed79-117">Application</span></span>|<span data-ttu-id="eed79-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eed79-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eed79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eed79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="eed79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eed79-120">Request headers</span></span>
|<span data-ttu-id="eed79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eed79-121">Header</span></span>|<span data-ttu-id="eed79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eed79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eed79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eed79-123">Authorization</span></span>|<span data-ttu-id="eed79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eed79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eed79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eed79-125">Accept</span></span>|<span data-ttu-id="eed79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eed79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eed79-127">Request body</span></span>
<span data-ttu-id="eed79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eed79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eed79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed79-129">Response</span></span>
<span data-ttu-id="eed79-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eed79-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed79-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed79-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eed79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed79-132">Request</span></span>
<span data-ttu-id="eed79-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eed79-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="eed79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed79-134">Response</span></span>
<span data-ttu-id="eed79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eed79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
      "label": "Label value",
      "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultItem": {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      },
      "items": [
        {
          "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
          "displayName": "Display Name value",
          "value": "Value value"
        }
      ],
      "required": true
    }
  ]
}
```





