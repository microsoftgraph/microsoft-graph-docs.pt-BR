---
title: Atualizar officeClientConfigurationAssignment
description: Atualiza as propriedades de um objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af97473ae7c72d3d107d2346e08caa7f264bc285
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420795"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="6aa49-103">Atualizar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6aa49-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="6aa49-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6aa49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aa49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6aa49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aa49-106">Atualiza as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6aa49-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aa49-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aa49-107">Prerequisites</span></span>
<span data-ttu-id="6aa49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa49-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aa49-110">Permission type</span></span>|<span data-ttu-id="6aa49-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6aa49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aa49-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aa49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa49-113">**TODO: Determine os escopos**</span><span class="sxs-lookup"><span data-stu-id="6aa49-113">**TODO: Determine scopes**</span></span>|
|<span data-ttu-id="6aa49-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aa49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aa49-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aa49-115">Not supported.</span></span>|
|<span data-ttu-id="6aa49-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aa49-116">Application</span></span>|<span data-ttu-id="6aa49-117">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="6aa49-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa49-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aa49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6aa49-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa49-119">Request headers</span></span>
|<span data-ttu-id="6aa49-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aa49-120">Header</span></span>|<span data-ttu-id="6aa49-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6aa49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aa49-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aa49-122">Authorization</span></span>|<span data-ttu-id="6aa49-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aa49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aa49-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aa49-124">Accept</span></span>|<span data-ttu-id="6aa49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa49-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa49-126">Request body</span></span>
<span data-ttu-id="6aa49-127">No corpo da solicitação, forneça uma representação JSON do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6aa49-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6aa49-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6aa49-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="6aa49-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aa49-129">Property</span></span>|<span data-ttu-id="6aa49-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aa49-130">Type</span></span>|<span data-ttu-id="6aa49-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aa49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aa49-132">id</span><span class="sxs-lookup"><span data-stu-id="6aa49-132">id</span></span>|<span data-ttu-id="6aa49-133">String</span><span class="sxs-lookup"><span data-stu-id="6aa49-133">String</span></span>|<span data-ttu-id="6aa49-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6aa49-134">Not yet documented</span></span>|
|<span data-ttu-id="6aa49-135">destino</span><span class="sxs-lookup"><span data-stu-id="6aa49-135">target</span></span>|[<span data-ttu-id="6aa49-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6aa49-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="6aa49-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6aa49-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6aa49-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aa49-138">Response</span></span>
<span data-ttu-id="6aa49-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aa49-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa49-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aa49-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aa49-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa49-141">Request</span></span>
<span data-ttu-id="6aa49-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aa49-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6aa49-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aa49-143">Response</span></span>
<span data-ttu-id="6aa49-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aa49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```






