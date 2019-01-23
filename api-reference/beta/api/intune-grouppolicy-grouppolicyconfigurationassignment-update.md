---
title: Atualizar groupPolicyConfigurationAssignment
description: Atualize as propriedades de um objeto groupPolicyConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08ff87b70b833dc1f8423a8465b5b880660fd462
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431292"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="9a94c-103">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9a94c-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="9a94c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a94c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a94c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a94c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a94c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a94c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a94c-107">Atualize as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9a94c-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a94c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a94c-108">Prerequisites</span></span>
<span data-ttu-id="9a94c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a94c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a94c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a94c-111">Permission type</span></span>|<span data-ttu-id="9a94c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a94c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a94c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a94c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a94c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a94c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a94c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a94c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a94c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a94c-116">Not supported.</span></span>|
|<span data-ttu-id="9a94c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a94c-117">Application</span></span>|<span data-ttu-id="9a94c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a94c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a94c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a94c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9a94c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a94c-120">Request headers</span></span>
|<span data-ttu-id="9a94c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a94c-121">Header</span></span>|<span data-ttu-id="9a94c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a94c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a94c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a94c-123">Authorization</span></span>|<span data-ttu-id="9a94c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a94c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a94c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a94c-125">Accept</span></span>|<span data-ttu-id="9a94c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a94c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a94c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a94c-127">Request body</span></span>
<span data-ttu-id="9a94c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9a94c-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="9a94c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9a94c-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="9a94c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a94c-130">Property</span></span>|<span data-ttu-id="9a94c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a94c-131">Type</span></span>|<span data-ttu-id="9a94c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a94c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a94c-133">id</span><span class="sxs-lookup"><span data-stu-id="9a94c-133">id</span></span>|<span data-ttu-id="9a94c-134">String</span><span class="sxs-lookup"><span data-stu-id="9a94c-134">String</span></span>|<span data-ttu-id="9a94c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a94c-135">Key of the entity.</span></span>|
|<span data-ttu-id="9a94c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a94c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9a94c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a94c-137">DateTimeOffset</span></span>|<span data-ttu-id="9a94c-138">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9a94c-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="9a94c-139">destino</span><span class="sxs-lookup"><span data-stu-id="9a94c-139">target</span></span>|[<span data-ttu-id="9a94c-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9a94c-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9a94c-141">O tipo de grupos direcionadas a configuração de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="9a94c-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="9a94c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a94c-142">Response</span></span>
<span data-ttu-id="9a94c-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a94c-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a94c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a94c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a94c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a94c-145">Request</span></span>
<span data-ttu-id="9a94c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a94c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9a94c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a94c-147">Response</span></span>
<span data-ttu-id="9a94c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a94c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




