---
title: Atualizar officeClientConfigurationAssignment
description: Atualiza as propriedades de um objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1125ab17915aaf56f5c5a334bd1775c1acf5be8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436747"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="589cc-103">Atualizar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="589cc-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="589cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="589cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="589cc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="589cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="589cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="589cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="589cc-107">Atualiza as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="589cc-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="589cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="589cc-108">Prerequisites</span></span>
<span data-ttu-id="589cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="589cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="589cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="589cc-111">Permission type</span></span>|<span data-ttu-id="589cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="589cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="589cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="589cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="589cc-114">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="589cc-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="589cc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="589cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="589cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="589cc-116">Not supported.</span></span>|
|<span data-ttu-id="589cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="589cc-117">Application</span></span>|<span data-ttu-id="589cc-118">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="589cc-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="589cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="589cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="589cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="589cc-120">Request headers</span></span>
|<span data-ttu-id="589cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="589cc-121">Header</span></span>|<span data-ttu-id="589cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="589cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="589cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="589cc-123">Authorization</span></span>|<span data-ttu-id="589cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="589cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="589cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="589cc-125">Accept</span></span>|<span data-ttu-id="589cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="589cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="589cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="589cc-127">Request body</span></span>
<span data-ttu-id="589cc-128">No corpo da solicitação, forneça uma representação JSON do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="589cc-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="589cc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="589cc-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="589cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="589cc-130">Property</span></span>|<span data-ttu-id="589cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="589cc-131">Type</span></span>|<span data-ttu-id="589cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="589cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="589cc-133">id</span><span class="sxs-lookup"><span data-stu-id="589cc-133">id</span></span>|<span data-ttu-id="589cc-134">String</span><span class="sxs-lookup"><span data-stu-id="589cc-134">String</span></span>|<span data-ttu-id="589cc-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="589cc-135">Not yet documented</span></span>|
|<span data-ttu-id="589cc-136">destino</span><span class="sxs-lookup"><span data-stu-id="589cc-136">target</span></span>|[<span data-ttu-id="589cc-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="589cc-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="589cc-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="589cc-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="589cc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="589cc-139">Response</span></span>
<span data-ttu-id="589cc-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="589cc-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="589cc-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="589cc-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="589cc-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="589cc-142">Request</span></span>
<span data-ttu-id="589cc-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="589cc-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="589cc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="589cc-144">Response</span></span>
<span data-ttu-id="589cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="589cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



