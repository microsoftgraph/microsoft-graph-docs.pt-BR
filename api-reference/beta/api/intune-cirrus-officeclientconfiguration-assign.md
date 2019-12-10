---
title: atribuir ação
description: Substituir todos os grupos de destino de uma política.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0eb257f51bdf6469fe08d3fe986ad9866bed9fc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930790"
---
# <a name="assign-action"></a><span data-ttu-id="e2e5d-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="e2e5d-103">assign action</span></span>

> <span data-ttu-id="e2e5d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2e5d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2e5d-106">Substituir todos os grupos de destino de uma política.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2e5d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2e5d-107">Prerequisites</span></span>
<span data-ttu-id="e2e5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2e5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e5d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2e5d-110">Permission type</span></span>|<span data-ttu-id="e2e5d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2e5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2e5d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2e5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2e5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2e5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2e5d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2e5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2e5d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-115">Not supported.</span></span>|
|<span data-ttu-id="e2e5d-116">Application</span><span class="sxs-lookup"><span data-stu-id="e2e5d-116">Application</span></span>|<span data-ttu-id="e2e5d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2e5d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2e5d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2e5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e2e5d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e5d-119">Request headers</span></span>
|<span data-ttu-id="e2e5d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2e5d-120">Header</span></span>|<span data-ttu-id="e2e5d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e2e5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2e5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2e5d-122">Authorization</span></span>|<span data-ttu-id="e2e5d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2e5d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2e5d-124">Accept</span></span>|<span data-ttu-id="e2e5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2e5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2e5d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e5d-126">Request body</span></span>
<span data-ttu-id="e2e5d-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e2e5d-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e2e5d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2e5d-129">Property</span></span>|<span data-ttu-id="e2e5d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2e5d-130">Type</span></span>|<span data-ttu-id="e2e5d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2e5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e5d-132">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="e2e5d-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="e2e5d-133">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e2e5d-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e2e5d-134">Lista de atribuições de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="e2e5d-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="e2e5d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2e5d-135">Response</span></span>
<span data-ttu-id="e2e5d-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2e5d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2e5d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2e5d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e5d-138">Request</span></span>
<span data-ttu-id="e2e5d-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e2e5d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2e5d-140">Response</span></span>
<span data-ttu-id="e2e5d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2e5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```





