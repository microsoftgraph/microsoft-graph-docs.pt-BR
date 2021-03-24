---
title: Atualizar termsAndConditions
description: Atualizar as propriedades de um objeto termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1d3b1120c60e20dbc0cc12cb27a903bcfd7c6b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133623"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="735e7-103">Atualizar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="735e7-103">Update termsAndConditions</span></span>

<span data-ttu-id="735e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="735e7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="735e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="735e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="735e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="735e7-107">Atualizar as propriedades de um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="735e7-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="735e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="735e7-108">Prerequisites</span></span>
<span data-ttu-id="735e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="735e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="735e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="735e7-111">Permission type</span></span>|<span data-ttu-id="735e7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="735e7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="735e7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="735e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="735e7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735e7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="735e7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="735e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="735e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="735e7-116">Not supported.</span></span>|
|<span data-ttu-id="735e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="735e7-117">Application</span></span>|<span data-ttu-id="735e7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735e7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="735e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="735e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="735e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="735e7-120">Request headers</span></span>
|<span data-ttu-id="735e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="735e7-121">Header</span></span>|<span data-ttu-id="735e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="735e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="735e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="735e7-123">Authorization</span></span>|<span data-ttu-id="735e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="735e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="735e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="735e7-125">Accept</span></span>|<span data-ttu-id="735e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="735e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="735e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="735e7-127">Request body</span></span>
<span data-ttu-id="735e7-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="735e7-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="735e7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="735e7-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="735e7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="735e7-130">Property</span></span>|<span data-ttu-id="735e7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="735e7-131">Type</span></span>|<span data-ttu-id="735e7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="735e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735e7-133">id</span><span class="sxs-lookup"><span data-stu-id="735e7-133">id</span></span>|<span data-ttu-id="735e7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="735e7-134">String</span></span>|<span data-ttu-id="735e7-135">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="735e7-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="735e7-136">createdDateTime</span></span>|<span data-ttu-id="735e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="735e7-137">DateTimeOffset</span></span>|<span data-ttu-id="735e7-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="735e7-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="735e7-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="735e7-139">modifiedDateTime</span></span>|<span data-ttu-id="735e7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="735e7-140">DateTimeOffset</span></span>|<span data-ttu-id="735e7-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="735e7-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="735e7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="735e7-142">lastModifiedDateTime</span></span>|<span data-ttu-id="735e7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="735e7-143">DateTimeOffset</span></span>|<span data-ttu-id="735e7-144">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="735e7-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="735e7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="735e7-145">displayName</span></span>|<span data-ttu-id="735e7-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="735e7-146">String</span></span>|<span data-ttu-id="735e7-147">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="735e7-148">descrição</span><span class="sxs-lookup"><span data-stu-id="735e7-148">description</span></span>|<span data-ttu-id="735e7-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="735e7-149">String</span></span>|<span data-ttu-id="735e7-150">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="735e7-151">title</span><span class="sxs-lookup"><span data-stu-id="735e7-151">title</span></span>|<span data-ttu-id="735e7-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="735e7-152">String</span></span>|<span data-ttu-id="735e7-153">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="735e7-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="735e7-154">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="735e7-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="735e7-155">bodyText</span></span>|<span data-ttu-id="735e7-156">String</span><span class="sxs-lookup"><span data-stu-id="735e7-156">String</span></span>|<span data-ttu-id="735e7-157">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="735e7-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="735e7-158">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="735e7-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="735e7-159">acceptanceStatement</span></span>|<span data-ttu-id="735e7-160">String</span><span class="sxs-lookup"><span data-stu-id="735e7-160">String</span></span>|<span data-ttu-id="735e7-161">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="735e7-162">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="735e7-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="735e7-163">version</span><span class="sxs-lookup"><span data-stu-id="735e7-163">version</span></span>|<span data-ttu-id="735e7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="735e7-164">Int32</span></span>|<span data-ttu-id="735e7-165">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="735e7-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="735e7-166">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="735e7-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="735e7-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="735e7-167">roleScopeTagIds</span></span>|<span data-ttu-id="735e7-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="735e7-168">String collection</span></span>|<span data-ttu-id="735e7-169">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="735e7-169">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="735e7-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="735e7-170">Response</span></span>
<span data-ttu-id="735e7-171">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="735e7-171">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="735e7-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="735e7-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="735e7-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="735e7-173">Request</span></span>
<span data-ttu-id="735e7-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="735e7-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="735e7-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="735e7-175">Response</span></span>
<span data-ttu-id="735e7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="735e7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




