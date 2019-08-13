---
title: Atualizar groupPolicyConfiguration
description: Atualiza as propriedades de um objeto groupPolicyConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07c13ca22db02707d9aa1ebc63085f0b824cb2b8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355301"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="0bc89-103">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0bc89-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="0bc89-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bc89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bc89-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bc89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bc89-106">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0bc89-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bc89-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bc89-107">Prerequisites</span></span>
<span data-ttu-id="0bc89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bc89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bc89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bc89-110">Permission type</span></span>|<span data-ttu-id="0bc89-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bc89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bc89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bc89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bc89-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bc89-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0bc89-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bc89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bc89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc89-115">Not supported.</span></span>|
|<span data-ttu-id="0bc89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bc89-116">Application</span></span>|<span data-ttu-id="0bc89-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bc89-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bc89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bc89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0bc89-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc89-119">Request headers</span></span>
|<span data-ttu-id="0bc89-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bc89-120">Header</span></span>|<span data-ttu-id="0bc89-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0bc89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bc89-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bc89-122">Authorization</span></span>|<span data-ttu-id="0bc89-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bc89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bc89-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bc89-124">Accept</span></span>|<span data-ttu-id="0bc89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bc89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc89-126">Request body</span></span>
<span data-ttu-id="0bc89-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0bc89-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="0bc89-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bc89-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="0bc89-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc89-129">Property</span></span>|<span data-ttu-id="0bc89-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc89-130">Type</span></span>|<span data-ttu-id="0bc89-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc89-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bc89-132">createdDateTime</span></span>|<span data-ttu-id="0bc89-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc89-133">DateTimeOffset</span></span>|<span data-ttu-id="0bc89-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0bc89-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="0bc89-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0bc89-135">displayName</span></span>|<span data-ttu-id="0bc89-136">String</span><span class="sxs-lookup"><span data-stu-id="0bc89-136">String</span></span>|<span data-ttu-id="0bc89-137">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="0bc89-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="0bc89-138">descrição</span><span class="sxs-lookup"><span data-stu-id="0bc89-138">description</span></span>|<span data-ttu-id="0bc89-139">String</span><span class="sxs-lookup"><span data-stu-id="0bc89-139">String</span></span>|<span data-ttu-id="0bc89-140">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="0bc89-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="0bc89-141">id</span><span class="sxs-lookup"><span data-stu-id="0bc89-141">id</span></span>|<span data-ttu-id="0bc89-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc89-142">String</span></span>|<span data-ttu-id="0bc89-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bc89-143">Key of the entity.</span></span>|
|<span data-ttu-id="0bc89-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bc89-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0bc89-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc89-145">DateTimeOffset</span></span>|<span data-ttu-id="0bc89-146">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0bc89-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0bc89-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc89-147">Response</span></span>
<span data-ttu-id="0bc89-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc89-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bc89-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bc89-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bc89-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc89-150">Request</span></span>
<span data-ttu-id="0bc89-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bc89-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="0bc89-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc89-152">Response</span></span>
<span data-ttu-id="0bc89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bc89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






