---
title: Criar termsAndConditions
description: Criar um novo objeto termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 972f0bbc19a7e9571ec85b643ef8d917a92a49ec
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170627"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="45017-103">Criar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="45017-103">Create termsAndConditions</span></span>

> <span data-ttu-id="45017-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45017-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45017-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45017-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45017-106">Criar um novo objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="45017-106">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45017-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45017-107">Prerequisites</span></span>
<span data-ttu-id="45017-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45017-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45017-110">Permission type</span></span>|<span data-ttu-id="45017-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45017-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45017-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45017-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45017-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45017-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45017-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45017-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45017-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45017-115">Not supported.</span></span>|
|<span data-ttu-id="45017-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45017-116">Application</span></span>|<span data-ttu-id="45017-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45017-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45017-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45017-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="45017-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45017-119">Request headers</span></span>
|<span data-ttu-id="45017-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45017-120">Header</span></span>|<span data-ttu-id="45017-121">Valor</span><span class="sxs-lookup"><span data-stu-id="45017-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45017-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="45017-122">Authorization</span></span>|<span data-ttu-id="45017-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45017-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45017-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45017-124">Accept</span></span>|<span data-ttu-id="45017-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45017-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45017-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45017-126">Request body</span></span>
<span data-ttu-id="45017-127">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="45017-127">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="45017-128">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="45017-128">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="45017-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45017-129">Property</span></span>|<span data-ttu-id="45017-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="45017-130">Type</span></span>|<span data-ttu-id="45017-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="45017-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45017-132">id</span><span class="sxs-lookup"><span data-stu-id="45017-132">id</span></span>|<span data-ttu-id="45017-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45017-133">String</span></span>|<span data-ttu-id="45017-134">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="45017-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45017-135">createdDateTime</span></span>|<span data-ttu-id="45017-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45017-136">DateTimeOffset</span></span>|<span data-ttu-id="45017-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45017-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="45017-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45017-138">modifiedDateTime</span></span>|<span data-ttu-id="45017-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45017-139">DateTimeOffset</span></span>|<span data-ttu-id="45017-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45017-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="45017-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45017-141">lastModifiedDateTime</span></span>|<span data-ttu-id="45017-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45017-142">DateTimeOffset</span></span>|<span data-ttu-id="45017-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45017-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="45017-144">displayName</span><span class="sxs-lookup"><span data-stu-id="45017-144">displayName</span></span>|<span data-ttu-id="45017-145">String</span><span class="sxs-lookup"><span data-stu-id="45017-145">String</span></span>|<span data-ttu-id="45017-146">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="45017-147">descrição</span><span class="sxs-lookup"><span data-stu-id="45017-147">description</span></span>|<span data-ttu-id="45017-148">String</span><span class="sxs-lookup"><span data-stu-id="45017-148">String</span></span>|<span data-ttu-id="45017-149">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="45017-150">title</span><span class="sxs-lookup"><span data-stu-id="45017-150">title</span></span>|<span data-ttu-id="45017-151">String</span><span class="sxs-lookup"><span data-stu-id="45017-151">String</span></span>|<span data-ttu-id="45017-152">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="45017-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="45017-153">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="45017-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="45017-154">bodyText</span></span>|<span data-ttu-id="45017-155">String</span><span class="sxs-lookup"><span data-stu-id="45017-155">String</span></span>|<span data-ttu-id="45017-156">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="45017-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="45017-157">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="45017-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="45017-158">acceptanceStatement</span></span>|<span data-ttu-id="45017-159">String</span><span class="sxs-lookup"><span data-stu-id="45017-159">String</span></span>|<span data-ttu-id="45017-160">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="45017-161">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="45017-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="45017-162">version</span><span class="sxs-lookup"><span data-stu-id="45017-162">version</span></span>|<span data-ttu-id="45017-163">Int32</span><span class="sxs-lookup"><span data-stu-id="45017-163">Int32</span></span>|<span data-ttu-id="45017-164">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="45017-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="45017-165">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="45017-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="45017-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45017-166">roleScopeTagIds</span></span>|<span data-ttu-id="45017-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45017-167">String collection</span></span>|<span data-ttu-id="45017-168">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="45017-168">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="45017-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="45017-169">Response</span></span>
<span data-ttu-id="45017-170">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45017-170">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45017-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45017-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="45017-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45017-172">Request</span></span>
<span data-ttu-id="45017-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45017-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45017-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="45017-174">Response</span></span>
<span data-ttu-id="45017-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45017-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




