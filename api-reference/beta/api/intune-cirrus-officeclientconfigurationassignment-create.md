---
title: Criar officeClientConfigurationAssignment
description: Adicione um grupo de destino a uma política existente.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3833115c1b652794e8d6b0557824389ebb974dd2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170852"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="49f06-103">Criar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f06-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="49f06-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49f06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49f06-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49f06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f06-106">Adicione um grupo de destino a uma política existente.</span><span class="sxs-lookup"><span data-stu-id="49f06-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49f06-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49f06-107">Prerequisites</span></span>
<span data-ttu-id="49f06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f06-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49f06-110">Permission type</span></span>|<span data-ttu-id="49f06-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49f06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f06-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49f06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49f06-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f06-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49f06-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49f06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f06-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49f06-115">Not supported.</span></span>|
|<span data-ttu-id="49f06-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49f06-116">Application</span></span>|<span data-ttu-id="49f06-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f06-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f06-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49f06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="49f06-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49f06-119">Request headers</span></span>
|<span data-ttu-id="49f06-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49f06-120">Header</span></span>|<span data-ttu-id="49f06-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49f06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49f06-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49f06-122">Authorization</span></span>|<span data-ttu-id="49f06-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49f06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49f06-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49f06-124">Accept</span></span>|<span data-ttu-id="49f06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49f06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f06-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49f06-126">Request body</span></span>
<span data-ttu-id="49f06-127">No corpo da solicitação, forneça uma representação JSON do objeto officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="49f06-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="49f06-128">A tabela a seguir mostra as propriedades que são necessárias ao criar officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="49f06-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="49f06-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49f06-129">Property</span></span>|<span data-ttu-id="49f06-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f06-130">Type</span></span>|<span data-ttu-id="49f06-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f06-132">id</span><span class="sxs-lookup"><span data-stu-id="49f06-132">id</span></span>|<span data-ttu-id="49f06-133">String</span><span class="sxs-lookup"><span data-stu-id="49f06-133">String</span></span>|<span data-ttu-id="49f06-134">ID do OfficeConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="49f06-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="49f06-135">destino</span><span class="sxs-lookup"><span data-stu-id="49f06-135">target</span></span>|[<span data-ttu-id="49f06-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="49f06-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="49f06-137">A atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="49f06-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="49f06-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f06-138">Response</span></span>
<span data-ttu-id="49f06-139">Se tiver êxito, este método retornará `200 Created` um código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49f06-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f06-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49f06-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="49f06-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49f06-141">Request</span></span>
<span data-ttu-id="49f06-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49f06-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="49f06-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f06-143">Response</span></span>
<span data-ttu-id="49f06-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




