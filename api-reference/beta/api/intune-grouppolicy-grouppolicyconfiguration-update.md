---
title: Atualizar groupPolicyConfiguration
description: Atualiza as propriedades de um objeto groupPolicyConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6265e7b9382322a138c39f05f57daa4579452a82
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804482"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="14b7f-103">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="14b7f-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="14b7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14b7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14b7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14b7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b7f-106">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14b7f-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14b7f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14b7f-107">Prerequisites</span></span>
<span data-ttu-id="14b7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b7f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14b7f-110">Permission type</span></span>|<span data-ttu-id="14b7f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14b7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b7f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14b7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14b7f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b7f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14b7f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14b7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b7f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14b7f-115">Not supported.</span></span>|
|<span data-ttu-id="14b7f-116">Application</span><span class="sxs-lookup"><span data-stu-id="14b7f-116">Application</span></span>|<span data-ttu-id="14b7f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b7f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b7f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14b7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14b7f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14b7f-119">Request headers</span></span>
|<span data-ttu-id="14b7f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14b7f-120">Header</span></span>|<span data-ttu-id="14b7f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14b7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b7f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14b7f-122">Authorization</span></span>|<span data-ttu-id="14b7f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14b7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b7f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14b7f-124">Accept</span></span>|<span data-ttu-id="14b7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14b7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b7f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14b7f-126">Request body</span></span>
<span data-ttu-id="14b7f-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14b7f-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="14b7f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14b7f-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="14b7f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14b7f-129">Property</span></span>|<span data-ttu-id="14b7f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="14b7f-130">Type</span></span>|<span data-ttu-id="14b7f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="14b7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b7f-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14b7f-132">createdDateTime</span></span>|<span data-ttu-id="14b7f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14b7f-133">DateTimeOffset</span></span>|<span data-ttu-id="14b7f-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="14b7f-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="14b7f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="14b7f-135">displayName</span></span>|<span data-ttu-id="14b7f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14b7f-136">String</span></span>|<span data-ttu-id="14b7f-137">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="14b7f-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="14b7f-138">description</span><span class="sxs-lookup"><span data-stu-id="14b7f-138">description</span></span>|<span data-ttu-id="14b7f-139">String</span><span class="sxs-lookup"><span data-stu-id="14b7f-139">String</span></span>|<span data-ttu-id="14b7f-140">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="14b7f-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="14b7f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14b7f-141">roleScopeTagIds</span></span>|<span data-ttu-id="14b7f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14b7f-142">String collection</span></span>|<span data-ttu-id="14b7f-143">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="14b7f-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="14b7f-144">id</span><span class="sxs-lookup"><span data-stu-id="14b7f-144">id</span></span>|<span data-ttu-id="14b7f-145">String</span><span class="sxs-lookup"><span data-stu-id="14b7f-145">String</span></span>|<span data-ttu-id="14b7f-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="14b7f-146">Key of the entity.</span></span>|
|<span data-ttu-id="14b7f-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14b7f-147">lastModifiedDateTime</span></span>|<span data-ttu-id="14b7f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14b7f-148">DateTimeOffset</span></span>|<span data-ttu-id="14b7f-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14b7f-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="14b7f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="14b7f-150">Response</span></span>
<span data-ttu-id="14b7f-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14b7f-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b7f-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14b7f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b7f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14b7f-153">Request</span></span>
<span data-ttu-id="14b7f-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14b7f-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14b7f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="14b7f-155">Response</span></span>
<span data-ttu-id="14b7f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14b7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




