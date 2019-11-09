---
title: Criar groupPolicyConfiguration
description: Criar um novo objeto groupPolicyConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01310fd9a04b96c0aef8a117bb314c4b1aaca7f9
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087100"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="692f2-103">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="692f2-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="692f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="692f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="692f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="692f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="692f2-106">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="692f2-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="692f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="692f2-107">Prerequisites</span></span>
<span data-ttu-id="692f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="692f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="692f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="692f2-110">Permission type</span></span>|<span data-ttu-id="692f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="692f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="692f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="692f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="692f2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="692f2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="692f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="692f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="692f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="692f2-115">Not supported.</span></span>|
|<span data-ttu-id="692f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="692f2-116">Application</span></span>|<span data-ttu-id="692f2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="692f2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="692f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="692f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="692f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="692f2-119">Request headers</span></span>
|<span data-ttu-id="692f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="692f2-120">Header</span></span>|<span data-ttu-id="692f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="692f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="692f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="692f2-122">Authorization</span></span>|<span data-ttu-id="692f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="692f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="692f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="692f2-124">Accept</span></span>|<span data-ttu-id="692f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="692f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="692f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="692f2-126">Request body</span></span>
<span data-ttu-id="692f2-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="692f2-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="692f2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="692f2-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="692f2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="692f2-129">Property</span></span>|<span data-ttu-id="692f2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="692f2-130">Type</span></span>|<span data-ttu-id="692f2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="692f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="692f2-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="692f2-132">createdDateTime</span></span>|<span data-ttu-id="692f2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="692f2-133">DateTimeOffset</span></span>|<span data-ttu-id="692f2-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="692f2-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="692f2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="692f2-135">displayName</span></span>|<span data-ttu-id="692f2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="692f2-136">String</span></span>|<span data-ttu-id="692f2-137">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="692f2-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="692f2-138">descrição</span><span class="sxs-lookup"><span data-stu-id="692f2-138">description</span></span>|<span data-ttu-id="692f2-139">String</span><span class="sxs-lookup"><span data-stu-id="692f2-139">String</span></span>|<span data-ttu-id="692f2-140">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="692f2-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="692f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="692f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="692f2-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="692f2-142">String collection</span></span>|<span data-ttu-id="692f2-143">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="692f2-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="692f2-144">id</span><span class="sxs-lookup"><span data-stu-id="692f2-144">id</span></span>|<span data-ttu-id="692f2-145">String</span><span class="sxs-lookup"><span data-stu-id="692f2-145">String</span></span>|<span data-ttu-id="692f2-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="692f2-146">Key of the entity.</span></span>|
|<span data-ttu-id="692f2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="692f2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="692f2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="692f2-148">DateTimeOffset</span></span>|<span data-ttu-id="692f2-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="692f2-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="692f2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="692f2-150">Response</span></span>
<span data-ttu-id="692f2-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="692f2-151">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="692f2-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="692f2-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="692f2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="692f2-153">Request</span></span>
<span data-ttu-id="692f2-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="692f2-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="692f2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="692f2-155">Response</span></span>
<span data-ttu-id="692f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="692f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






