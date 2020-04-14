---
title: Atualizar groupPolicyConfiguration
description: Atualiza as propriedades de um objeto groupPolicyConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3a261947073c96934cc6c84c276fc232d06c0b1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454662"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="14c67-103">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="14c67-103">Update groupPolicyConfiguration</span></span>

<span data-ttu-id="14c67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14c67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14c67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14c67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14c67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14c67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14c67-107">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14c67-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14c67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14c67-108">Prerequisites</span></span>
<span data-ttu-id="14c67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14c67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14c67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14c67-111">Permission type</span></span>|<span data-ttu-id="14c67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14c67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14c67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14c67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14c67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14c67-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14c67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14c67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14c67-116">Not supported.</span></span>|
|<span data-ttu-id="14c67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14c67-117">Application</span></span>|<span data-ttu-id="14c67-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c67-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14c67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14c67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14c67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14c67-120">Request headers</span></span>
|<span data-ttu-id="14c67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14c67-121">Header</span></span>|<span data-ttu-id="14c67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14c67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14c67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14c67-123">Authorization</span></span>|<span data-ttu-id="14c67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14c67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14c67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14c67-125">Accept</span></span>|<span data-ttu-id="14c67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14c67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14c67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14c67-127">Request body</span></span>
<span data-ttu-id="14c67-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14c67-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="14c67-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14c67-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="14c67-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14c67-130">Property</span></span>|<span data-ttu-id="14c67-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="14c67-131">Type</span></span>|<span data-ttu-id="14c67-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14c67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14c67-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14c67-133">createdDateTime</span></span>|<span data-ttu-id="14c67-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14c67-134">DateTimeOffset</span></span>|<span data-ttu-id="14c67-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="14c67-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="14c67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="14c67-136">displayName</span></span>|<span data-ttu-id="14c67-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14c67-137">String</span></span>|<span data-ttu-id="14c67-138">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="14c67-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="14c67-139">description</span><span class="sxs-lookup"><span data-stu-id="14c67-139">description</span></span>|<span data-ttu-id="14c67-140">String</span><span class="sxs-lookup"><span data-stu-id="14c67-140">String</span></span>|<span data-ttu-id="14c67-141">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="14c67-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="14c67-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14c67-142">roleScopeTagIds</span></span>|<span data-ttu-id="14c67-143">Coleção String</span><span class="sxs-lookup"><span data-stu-id="14c67-143">String collection</span></span>|<span data-ttu-id="14c67-144">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="14c67-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="14c67-145">id</span><span class="sxs-lookup"><span data-stu-id="14c67-145">id</span></span>|<span data-ttu-id="14c67-146">String</span><span class="sxs-lookup"><span data-stu-id="14c67-146">String</span></span>|<span data-ttu-id="14c67-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="14c67-147">Key of the entity.</span></span>|
|<span data-ttu-id="14c67-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14c67-148">lastModifiedDateTime</span></span>|<span data-ttu-id="14c67-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14c67-149">DateTimeOffset</span></span>|<span data-ttu-id="14c67-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14c67-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="14c67-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="14c67-151">Response</span></span>
<span data-ttu-id="14c67-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14c67-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14c67-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14c67-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="14c67-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14c67-154">Request</span></span>
<span data-ttu-id="14c67-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14c67-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
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

### <a name="response"></a><span data-ttu-id="14c67-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="14c67-156">Response</span></span>
<span data-ttu-id="14c67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14c67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



