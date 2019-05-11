---
title: Listar officeClientConfigurationAssignments
description: Listar Propriedades e relações dos objetos officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: b7b5eeac4c0a07d4cf4e87401a6e0bbf3b11aaf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934009"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="29377-103">Listar officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="29377-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="29377-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29377-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29377-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29377-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29377-106">Listar Propriedades e relações dos objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="29377-106">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29377-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29377-107">Prerequisites</span></span>
<span data-ttu-id="29377-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29377-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29377-110">Permission type</span></span>|<span data-ttu-id="29377-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29377-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29377-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29377-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29377-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="29377-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="29377-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29377-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29377-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29377-115">Not supported.</span></span>|
|<span data-ttu-id="29377-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29377-116">Application</span></span>|<span data-ttu-id="29377-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29377-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29377-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29377-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="29377-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29377-119">Request headers</span></span>
|<span data-ttu-id="29377-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29377-120">Header</span></span>|<span data-ttu-id="29377-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29377-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29377-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29377-122">Authorization</span></span>|<span data-ttu-id="29377-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29377-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29377-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29377-124">Accept</span></span>|<span data-ttu-id="29377-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29377-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29377-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29377-126">Request body</span></span>
<span data-ttu-id="29377-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29377-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29377-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="29377-128">Response</span></span>
<span data-ttu-id="29377-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29377-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29377-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29377-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="29377-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29377-131">Request</span></span>
<span data-ttu-id="29377-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29377-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="29377-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="29377-133">Response</span></span>
<span data-ttu-id="29377-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29377-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



