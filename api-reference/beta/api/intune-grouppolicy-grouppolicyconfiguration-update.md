---
title: Atualizar groupPolicyConfiguration
description: Atualize as propriedades de um objeto groupPolicyConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 294bf20454e597f95d607b04abcdfaa6bd3d4a25
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153395"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="a16db-103">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="a16db-103">Update groupPolicyConfiguration</span></span>

<span data-ttu-id="a16db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a16db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a16db-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a16db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a16db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a16db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a16db-107">Atualize as propriedades de [um objeto groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a16db-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a16db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a16db-108">Prerequisites</span></span>
<span data-ttu-id="a16db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a16db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a16db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a16db-111">Permission type</span></span>|<span data-ttu-id="a16db-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a16db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a16db-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a16db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a16db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a16db-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a16db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a16db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a16db-116">Not supported.</span></span>|
|<span data-ttu-id="a16db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a16db-117">Application</span></span>|<span data-ttu-id="a16db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a16db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a16db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a16db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a16db-120">Request headers</span></span>
|<span data-ttu-id="a16db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a16db-121">Header</span></span>|<span data-ttu-id="a16db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a16db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a16db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a16db-123">Authorization</span></span>|<span data-ttu-id="a16db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a16db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a16db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a16db-125">Accept</span></span>|<span data-ttu-id="a16db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a16db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a16db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a16db-127">Request body</span></span>
<span data-ttu-id="a16db-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a16db-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="a16db-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a16db-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="a16db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a16db-130">Property</span></span>|<span data-ttu-id="a16db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a16db-131">Type</span></span>|<span data-ttu-id="a16db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a16db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a16db-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a16db-133">createdDateTime</span></span>|<span data-ttu-id="a16db-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16db-134">DateTimeOffset</span></span>|<span data-ttu-id="a16db-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a16db-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="a16db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a16db-136">displayName</span></span>|<span data-ttu-id="a16db-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a16db-137">String</span></span>|<span data-ttu-id="a16db-138">Nome fornecido pelo usuário para o objeto resource.</span><span class="sxs-lookup"><span data-stu-id="a16db-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="a16db-139">descrição</span><span class="sxs-lookup"><span data-stu-id="a16db-139">description</span></span>|<span data-ttu-id="a16db-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a16db-140">String</span></span>|<span data-ttu-id="a16db-141">O usuário forneceu a descrição do objeto resource.</span><span class="sxs-lookup"><span data-stu-id="a16db-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="a16db-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a16db-142">roleScopeTagIds</span></span>|<span data-ttu-id="a16db-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a16db-143">String collection</span></span>|<span data-ttu-id="a16db-144">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="a16db-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="a16db-145">id</span><span class="sxs-lookup"><span data-stu-id="a16db-145">id</span></span>|<span data-ttu-id="a16db-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a16db-146">String</span></span>|<span data-ttu-id="a16db-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a16db-147">Key of the entity.</span></span>|
|<span data-ttu-id="a16db-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a16db-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a16db-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16db-149">DateTimeOffset</span></span>|<span data-ttu-id="a16db-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a16db-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a16db-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a16db-151">Response</span></span>
<span data-ttu-id="a16db-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a16db-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a16db-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a16db-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a16db-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a16db-154">Request</span></span>
<span data-ttu-id="a16db-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a16db-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a16db-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a16db-156">Response</span></span>
<span data-ttu-id="a16db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a16db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




