---
title: Criar termsAndConditions
description: Criar um novo objeto termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 410b74df44bfbed8a61b68db0e89364b550bf465
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695849"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="1c0a3-103">Criar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1c0a3-103">Create termsAndConditions</span></span>

<span data-ttu-id="1c0a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c0a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c0a3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c0a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c0a3-107">Criar um novo objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c0a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c0a3-108">Prerequisites</span></span>
<span data-ttu-id="1c0a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c0a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c0a3-111">Permission type</span></span>|<span data-ttu-id="1c0a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c0a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c0a3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c0a3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c0a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c0a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-116">Not supported.</span></span>|
|<span data-ttu-id="1c0a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-117">Application</span></span>|<span data-ttu-id="1c0a3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c0a3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c0a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c0a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="1c0a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-120">Request headers</span></span>
|<span data-ttu-id="1c0a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c0a3-121">Header</span></span>|<span data-ttu-id="1c0a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c0a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c0a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c0a3-123">Authorization</span></span>|<span data-ttu-id="1c0a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c0a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c0a3-125">Accept</span></span>|<span data-ttu-id="1c0a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c0a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c0a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-127">Request body</span></span>
<span data-ttu-id="1c0a3-128">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="1c0a3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="1c0a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c0a3-130">Property</span></span>|<span data-ttu-id="1c0a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-131">Type</span></span>|<span data-ttu-id="1c0a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c0a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c0a3-133">id</span><span class="sxs-lookup"><span data-stu-id="1c0a3-133">id</span></span>|<span data-ttu-id="1c0a3-134">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-134">String</span></span>|<span data-ttu-id="1c0a3-135">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c0a3-136">createdDateTime</span></span>|<span data-ttu-id="1c0a3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c0a3-137">DateTimeOffset</span></span>|<span data-ttu-id="1c0a3-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="1c0a3-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c0a3-139">modifiedDateTime</span></span>|<span data-ttu-id="1c0a3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c0a3-140">DateTimeOffset</span></span>|<span data-ttu-id="1c0a3-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1c0a3-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c0a3-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1c0a3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c0a3-143">DateTimeOffset</span></span>|<span data-ttu-id="1c0a3-144">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1c0a3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1c0a3-145">displayName</span></span>|<span data-ttu-id="1c0a3-146">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-146">String</span></span>|<span data-ttu-id="1c0a3-147">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="1c0a3-148">description</span><span class="sxs-lookup"><span data-stu-id="1c0a3-148">description</span></span>|<span data-ttu-id="1c0a3-149">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-149">String</span></span>|<span data-ttu-id="1c0a3-150">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-151">title</span><span class="sxs-lookup"><span data-stu-id="1c0a3-151">title</span></span>|<span data-ttu-id="1c0a3-152">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-152">String</span></span>|<span data-ttu-id="1c0a3-153">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="1c0a3-154">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="1c0a3-155">bodyText</span></span>|<span data-ttu-id="1c0a3-156">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-156">String</span></span>|<span data-ttu-id="1c0a3-157">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="1c0a3-158">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="1c0a3-159">acceptanceStatement</span></span>|<span data-ttu-id="1c0a3-160">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-160">String</span></span>|<span data-ttu-id="1c0a3-161">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="1c0a3-162">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-163">version</span><span class="sxs-lookup"><span data-stu-id="1c0a3-163">version</span></span>|<span data-ttu-id="1c0a3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1c0a3-164">Int32</span></span>|<span data-ttu-id="1c0a3-165">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="1c0a3-166">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="1c0a3-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c0a3-167">roleScopeTagIds</span></span>|<span data-ttu-id="1c0a3-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c0a3-168">String collection</span></span>|<span data-ttu-id="1c0a3-169">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-169">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1c0a3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c0a3-170">Response</span></span>
<span data-ttu-id="1c0a3-171">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-171">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c0a3-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c0a3-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-173">Request</span></span>
<span data-ttu-id="1c0a3-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1c0a3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c0a3-175">Response</span></span>
<span data-ttu-id="1c0a3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





