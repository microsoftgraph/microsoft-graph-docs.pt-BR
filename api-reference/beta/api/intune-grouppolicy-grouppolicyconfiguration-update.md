---
title: Atualizar groupPolicyConfiguration
description: Atualize as propriedades de um objeto groupPolicyConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30ce815eef79de3fa091daede34c758699f27bc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429238"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="48f19-103">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48f19-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="48f19-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="48f19-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48f19-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48f19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48f19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="48f19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f19-107">Atualize as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48f19-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48f19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48f19-108">Prerequisites</span></span>
<span data-ttu-id="48f19-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48f19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48f19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48f19-111">Permission type</span></span>|<span data-ttu-id="48f19-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48f19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48f19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48f19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48f19-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f19-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48f19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48f19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48f19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f19-116">Not supported.</span></span>|
|<span data-ttu-id="48f19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48f19-117">Application</span></span>|<span data-ttu-id="48f19-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48f19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48f19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="48f19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48f19-120">Request headers</span></span>
|<span data-ttu-id="48f19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48f19-121">Header</span></span>|<span data-ttu-id="48f19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48f19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48f19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48f19-123">Authorization</span></span>|<span data-ttu-id="48f19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48f19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48f19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48f19-125">Accept</span></span>|<span data-ttu-id="48f19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48f19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48f19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48f19-127">Request body</span></span>
<span data-ttu-id="48f19-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48f19-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="48f19-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48f19-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="48f19-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48f19-130">Property</span></span>|<span data-ttu-id="48f19-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f19-131">Type</span></span>|<span data-ttu-id="48f19-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f19-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48f19-133">createdDateTime</span></span>|<span data-ttu-id="48f19-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48f19-134">DateTimeOffset</span></span>|<span data-ttu-id="48f19-135">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="48f19-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="48f19-136">displayName</span><span class="sxs-lookup"><span data-stu-id="48f19-136">displayName</span></span>|<span data-ttu-id="48f19-137">String</span><span class="sxs-lookup"><span data-stu-id="48f19-137">String</span></span>|<span data-ttu-id="48f19-138">Nome de usuário fornecido para o objeto resource.</span><span class="sxs-lookup"><span data-stu-id="48f19-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="48f19-139">description</span><span class="sxs-lookup"><span data-stu-id="48f19-139">description</span></span>|<span data-ttu-id="48f19-140">String</span><span class="sxs-lookup"><span data-stu-id="48f19-140">String</span></span>|<span data-ttu-id="48f19-141">Descrição para o objeto resource fornecidos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="48f19-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="48f19-142">id</span><span class="sxs-lookup"><span data-stu-id="48f19-142">id</span></span>|<span data-ttu-id="48f19-143">String</span><span class="sxs-lookup"><span data-stu-id="48f19-143">String</span></span>|<span data-ttu-id="48f19-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48f19-144">Key of the entity.</span></span>|
|<span data-ttu-id="48f19-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48f19-145">lastModifiedDateTime</span></span>|<span data-ttu-id="48f19-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48f19-146">DateTimeOffset</span></span>|<span data-ttu-id="48f19-147">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="48f19-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="48f19-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f19-148">Response</span></span>
<span data-ttu-id="48f19-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48f19-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48f19-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48f19-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="48f19-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48f19-151">Request</span></span>
<span data-ttu-id="48f19-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48f19-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48f19-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f19-153">Response</span></span>
<span data-ttu-id="48f19-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48f19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




