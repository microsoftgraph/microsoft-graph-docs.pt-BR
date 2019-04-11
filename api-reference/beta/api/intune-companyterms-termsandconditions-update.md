---
title: Atualizar termsAndConditions
description: Atualizar as propriedades de um objeto termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cc6eb5a3ad5b129693fa5bbedf55c56252bf19b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780550"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="49d4a-103">Atualizar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="49d4a-103">Update termsAndConditions</span></span>

> <span data-ttu-id="49d4a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49d4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49d4a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49d4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49d4a-106">Atualizar as propriedades de um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="49d4a-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49d4a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49d4a-107">Prerequisites</span></span>
<span data-ttu-id="49d4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d4a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49d4a-110">Permission type</span></span>|<span data-ttu-id="49d4a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49d4a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49d4a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49d4a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49d4a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49d4a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49d4a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49d4a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49d4a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49d4a-115">Not supported.</span></span>|
|<span data-ttu-id="49d4a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49d4a-116">Application</span></span>|<span data-ttu-id="49d4a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49d4a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49d4a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49d4a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="49d4a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49d4a-119">Request headers</span></span>
|<span data-ttu-id="49d4a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49d4a-120">Header</span></span>|<span data-ttu-id="49d4a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49d4a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49d4a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49d4a-122">Authorization</span></span>|<span data-ttu-id="49d4a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d4a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49d4a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49d4a-124">Accept</span></span>|<span data-ttu-id="49d4a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49d4a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49d4a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49d4a-126">Request body</span></span>
<span data-ttu-id="49d4a-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="49d4a-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="49d4a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="49d4a-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="49d4a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49d4a-129">Property</span></span>|<span data-ttu-id="49d4a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49d4a-130">Type</span></span>|<span data-ttu-id="49d4a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49d4a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d4a-132">id</span><span class="sxs-lookup"><span data-stu-id="49d4a-132">id</span></span>|<span data-ttu-id="49d4a-133">String</span><span class="sxs-lookup"><span data-stu-id="49d4a-133">String</span></span>|<span data-ttu-id="49d4a-134">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="49d4a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49d4a-135">createdDateTime</span></span>|<span data-ttu-id="49d4a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49d4a-136">DateTimeOffset</span></span>|<span data-ttu-id="49d4a-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="49d4a-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="49d4a-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49d4a-138">modifiedDateTime</span></span>|<span data-ttu-id="49d4a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49d4a-139">DateTimeOffset</span></span>|<span data-ttu-id="49d4a-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="49d4a-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="49d4a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49d4a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="49d4a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49d4a-142">DateTimeOffset</span></span>|<span data-ttu-id="49d4a-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="49d4a-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="49d4a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="49d4a-144">displayName</span></span>|<span data-ttu-id="49d4a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49d4a-145">String</span></span>|<span data-ttu-id="49d4a-146">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="49d4a-147">description</span><span class="sxs-lookup"><span data-stu-id="49d4a-147">description</span></span>|<span data-ttu-id="49d4a-148">String</span><span class="sxs-lookup"><span data-stu-id="49d4a-148">String</span></span>|<span data-ttu-id="49d4a-149">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="49d4a-150">title</span><span class="sxs-lookup"><span data-stu-id="49d4a-150">title</span></span>|<span data-ttu-id="49d4a-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49d4a-151">String</span></span>|<span data-ttu-id="49d4a-152">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="49d4a-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="49d4a-153">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="49d4a-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="49d4a-154">bodyText</span></span>|<span data-ttu-id="49d4a-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49d4a-155">String</span></span>|<span data-ttu-id="49d4a-156">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="49d4a-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="49d4a-157">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="49d4a-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="49d4a-158">acceptanceStatement</span></span>|<span data-ttu-id="49d4a-159">String</span><span class="sxs-lookup"><span data-stu-id="49d4a-159">String</span></span>|<span data-ttu-id="49d4a-160">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="49d4a-161">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="49d4a-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="49d4a-162">version</span><span class="sxs-lookup"><span data-stu-id="49d4a-162">version</span></span>|<span data-ttu-id="49d4a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="49d4a-163">Int32</span></span>|<span data-ttu-id="49d4a-164">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="49d4a-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="49d4a-165">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="49d4a-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="49d4a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="49d4a-166">Response</span></span>
<span data-ttu-id="49d4a-167">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49d4a-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49d4a-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49d4a-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="49d4a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49d4a-169">Request</span></span>
<span data-ttu-id="49d4a-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49d4a-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="49d4a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="49d4a-171">Response</span></span>
<span data-ttu-id="49d4a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49d4a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

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
  "version": 7
}
```





