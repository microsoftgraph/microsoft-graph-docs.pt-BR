---
title: Atualizar officeClientConfigurationAssignment
description: Atualiza as propriedades de um objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 280e1e6d834cd7a9692c75d01434f97f9cba740c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322202"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="3f673-103">Atualizar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3f673-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="3f673-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f673-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f673-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f673-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f673-106">Atualiza as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3f673-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f673-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f673-107">Prerequisites</span></span>
<span data-ttu-id="3f673-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f673-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f673-110">Permission type</span></span>|<span data-ttu-id="3f673-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f673-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f673-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f673-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f673-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="3f673-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="3f673-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f673-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f673-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f673-115">Not supported.</span></span>|
|<span data-ttu-id="3f673-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f673-116">Application</span></span>|<span data-ttu-id="3f673-117">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="3f673-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f673-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f673-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3f673-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f673-119">Request headers</span></span>
|<span data-ttu-id="3f673-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f673-120">Header</span></span>|<span data-ttu-id="3f673-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3f673-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f673-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f673-122">Authorization</span></span>|<span data-ttu-id="3f673-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f673-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f673-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f673-124">Accept</span></span>|<span data-ttu-id="3f673-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f673-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f673-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f673-126">Request body</span></span>
<span data-ttu-id="3f673-127">No corpo da solicitação, forneça uma representação JSON do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3f673-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="3f673-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3f673-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="3f673-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f673-129">Property</span></span>|<span data-ttu-id="3f673-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f673-130">Type</span></span>|<span data-ttu-id="3f673-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f673-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f673-132">id</span><span class="sxs-lookup"><span data-stu-id="3f673-132">id</span></span>|<span data-ttu-id="3f673-133">String</span><span class="sxs-lookup"><span data-stu-id="3f673-133">String</span></span>|<span data-ttu-id="3f673-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3f673-134">Not yet documented</span></span>|
|<span data-ttu-id="3f673-135">destino</span><span class="sxs-lookup"><span data-stu-id="3f673-135">target</span></span>|[<span data-ttu-id="3f673-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3f673-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="3f673-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3f673-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f673-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f673-138">Response</span></span>
<span data-ttu-id="3f673-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f673-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f673-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f673-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f673-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f673-141">Request</span></span>
<span data-ttu-id="3f673-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f673-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f673-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f673-143">Response</span></span>
<span data-ttu-id="3f673-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f673-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






