---
title: Criar groupPolicyConfiguration
description: Criar um novo objeto groupPolicyConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec6bbb8353c8f39ed5249fca909b8387d9cb2104
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973303"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="7215c-103">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="7215c-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="7215c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7215c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7215c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7215c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7215c-106">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7215c-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7215c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7215c-107">Prerequisites</span></span>
<span data-ttu-id="7215c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7215c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7215c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7215c-110">Permission type</span></span>|<span data-ttu-id="7215c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7215c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7215c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7215c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7215c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7215c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7215c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7215c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7215c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7215c-115">Not supported.</span></span>|
|<span data-ttu-id="7215c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7215c-116">Application</span></span>|<span data-ttu-id="7215c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7215c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7215c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7215c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7215c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7215c-119">Request headers</span></span>
|<span data-ttu-id="7215c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7215c-120">Header</span></span>|<span data-ttu-id="7215c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7215c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7215c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7215c-122">Authorization</span></span>|<span data-ttu-id="7215c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7215c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7215c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7215c-124">Accept</span></span>|<span data-ttu-id="7215c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7215c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7215c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7215c-126">Request body</span></span>
<span data-ttu-id="7215c-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7215c-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="7215c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7215c-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="7215c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7215c-129">Property</span></span>|<span data-ttu-id="7215c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7215c-130">Type</span></span>|<span data-ttu-id="7215c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7215c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7215c-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7215c-132">createdDateTime</span></span>|<span data-ttu-id="7215c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7215c-133">DateTimeOffset</span></span>|<span data-ttu-id="7215c-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7215c-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="7215c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7215c-135">displayName</span></span>|<span data-ttu-id="7215c-136">String</span><span class="sxs-lookup"><span data-stu-id="7215c-136">String</span></span>|<span data-ttu-id="7215c-137">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="7215c-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="7215c-138">descrição</span><span class="sxs-lookup"><span data-stu-id="7215c-138">description</span></span>|<span data-ttu-id="7215c-139">String</span><span class="sxs-lookup"><span data-stu-id="7215c-139">String</span></span>|<span data-ttu-id="7215c-140">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="7215c-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="7215c-141">id</span><span class="sxs-lookup"><span data-stu-id="7215c-141">id</span></span>|<span data-ttu-id="7215c-142">String</span><span class="sxs-lookup"><span data-stu-id="7215c-142">String</span></span>|<span data-ttu-id="7215c-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7215c-143">Key of the entity.</span></span>|
|<span data-ttu-id="7215c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7215c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="7215c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7215c-145">DateTimeOffset</span></span>|<span data-ttu-id="7215c-146">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7215c-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="7215c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7215c-147">Response</span></span>
<span data-ttu-id="7215c-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7215c-148">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7215c-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7215c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7215c-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7215c-150">Request</span></span>
<span data-ttu-id="7215c-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7215c-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="7215c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7215c-152">Response</span></span>
<span data-ttu-id="7215c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7215c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




