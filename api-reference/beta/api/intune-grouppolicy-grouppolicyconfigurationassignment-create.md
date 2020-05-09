---
title: Criar groupPolicyConfigurationAssignment
description: Criar um novo objeto groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a8cd32323145cf0148b6d2be4dd93ee3e3471b8
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178371"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="ae524-103">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ae524-103">Create groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="ae524-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae524-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae524-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae524-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae524-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae524-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae524-107">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ae524-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae524-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae524-108">Prerequisites</span></span>
<span data-ttu-id="ae524-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae524-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae524-111">Permission type</span></span>|<span data-ttu-id="ae524-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae524-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae524-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae524-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae524-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae524-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae524-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae524-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae524-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae524-116">Not supported.</span></span>|
|<span data-ttu-id="ae524-117">Application</span><span class="sxs-lookup"><span data-stu-id="ae524-117">Application</span></span>|<span data-ttu-id="ae524-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae524-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae524-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae524-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ae524-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae524-120">Request headers</span></span>
|<span data-ttu-id="ae524-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae524-121">Header</span></span>|<span data-ttu-id="ae524-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae524-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae524-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae524-123">Authorization</span></span>|<span data-ttu-id="ae524-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae524-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae524-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae524-125">Accept</span></span>|<span data-ttu-id="ae524-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae524-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae524-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae524-127">Request body</span></span>
<span data-ttu-id="ae524-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ae524-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="ae524-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ae524-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="ae524-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae524-130">Property</span></span>|<span data-ttu-id="ae524-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae524-131">Type</span></span>|<span data-ttu-id="ae524-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae524-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae524-133">id</span><span class="sxs-lookup"><span data-stu-id="ae524-133">id</span></span>|<span data-ttu-id="ae524-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae524-134">String</span></span>|<span data-ttu-id="ae524-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae524-135">Key of the entity.</span></span>|
|<span data-ttu-id="ae524-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae524-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ae524-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae524-137">DateTimeOffset</span></span>|<span data-ttu-id="ae524-138">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae524-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="ae524-139">destino</span><span class="sxs-lookup"><span data-stu-id="ae524-139">target</span></span>|[<span data-ttu-id="ae524-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ae524-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ae524-141">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="ae524-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ae524-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae524-142">Response</span></span>
<span data-ttu-id="ae524-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae524-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae524-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae524-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae524-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae524-145">Request</span></span>
<span data-ttu-id="ae524-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae524-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ae524-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae524-147">Response</span></span>
<span data-ttu-id="ae524-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae524-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



