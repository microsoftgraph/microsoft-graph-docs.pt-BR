---
title: Criar groupPolicyConfiguration
description: Criar um novo objeto groupPolicyConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bfb9d75b373867dcefa4625ab2cc46e9a5c9e0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465279"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="22500-103">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="22500-103">Create groupPolicyConfiguration</span></span>

<span data-ttu-id="22500-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22500-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22500-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22500-107">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="22500-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22500-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22500-108">Prerequisites</span></span>
<span data-ttu-id="22500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22500-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22500-111">Permission type</span></span>|<span data-ttu-id="22500-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22500-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22500-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22500-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22500-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22500-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22500-116">Not supported.</span></span>|
|<span data-ttu-id="22500-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22500-117">Application</span></span>|<span data-ttu-id="22500-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22500-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22500-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22500-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22500-120">Request headers</span></span>
|<span data-ttu-id="22500-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22500-121">Header</span></span>|<span data-ttu-id="22500-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22500-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22500-123">Authorization</span></span>|<span data-ttu-id="22500-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22500-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22500-125">Accept</span></span>|<span data-ttu-id="22500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22500-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22500-127">Request body</span></span>
<span data-ttu-id="22500-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22500-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="22500-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22500-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="22500-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22500-130">Property</span></span>|<span data-ttu-id="22500-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22500-131">Type</span></span>|<span data-ttu-id="22500-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22500-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22500-133">createdDateTime</span></span>|<span data-ttu-id="22500-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22500-134">DateTimeOffset</span></span>|<span data-ttu-id="22500-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22500-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="22500-136">displayName</span><span class="sxs-lookup"><span data-stu-id="22500-136">displayName</span></span>|<span data-ttu-id="22500-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22500-137">String</span></span>|<span data-ttu-id="22500-138">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="22500-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="22500-139">description</span><span class="sxs-lookup"><span data-stu-id="22500-139">description</span></span>|<span data-ttu-id="22500-140">String</span><span class="sxs-lookup"><span data-stu-id="22500-140">String</span></span>|<span data-ttu-id="22500-141">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="22500-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="22500-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22500-142">roleScopeTagIds</span></span>|<span data-ttu-id="22500-143">String collection</span><span class="sxs-lookup"><span data-stu-id="22500-143">String collection</span></span>|<span data-ttu-id="22500-144">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="22500-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="22500-145">id</span><span class="sxs-lookup"><span data-stu-id="22500-145">id</span></span>|<span data-ttu-id="22500-146">String</span><span class="sxs-lookup"><span data-stu-id="22500-146">String</span></span>|<span data-ttu-id="22500-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22500-147">Key of the entity.</span></span>|
|<span data-ttu-id="22500-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22500-148">lastModifiedDateTime</span></span>|<span data-ttu-id="22500-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22500-149">DateTimeOffset</span></span>|<span data-ttu-id="22500-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="22500-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="22500-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="22500-151">Response</span></span>
<span data-ttu-id="22500-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22500-152">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22500-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22500-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="22500-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22500-154">Request</span></span>
<span data-ttu-id="22500-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22500-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22500-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="22500-156">Response</span></span>
<span data-ttu-id="22500-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22500-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





