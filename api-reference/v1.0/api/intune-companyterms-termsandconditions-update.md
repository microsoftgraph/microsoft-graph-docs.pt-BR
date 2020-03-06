---
title: Atualizar termsAndConditions
description: Atualizar as propriedades de um objeto termsAndConditions.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f863a9e7f0235a34a03ceb36f931f6cfb9514ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515473"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="a2e62-103">Atualizar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a2e62-103">Update termsAndConditions</span></span>

<span data-ttu-id="a2e62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2e62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2e62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e62-106">Atualizar as propriedades de um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a2e62-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2e62-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2e62-107">Prerequisites</span></span>
<span data-ttu-id="a2e62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2e62-110">Permission type</span></span>|<span data-ttu-id="a2e62-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2e62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2e62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e62-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e62-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2e62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2e62-115">Not supported.</span></span>|
|<span data-ttu-id="a2e62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2e62-116">Application</span></span>|<span data-ttu-id="a2e62-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2e62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2e62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="a2e62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e62-119">Request headers</span></span>
|<span data-ttu-id="a2e62-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2e62-120">Header</span></span>|<span data-ttu-id="a2e62-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2e62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2e62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2e62-122">Authorization</span></span>|<span data-ttu-id="a2e62-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2e62-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2e62-124">Accept</span></span>|<span data-ttu-id="a2e62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2e62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e62-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e62-126">Request body</span></span>
<span data-ttu-id="a2e62-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a2e62-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="a2e62-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a2e62-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="a2e62-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2e62-129">Property</span></span>|<span data-ttu-id="a2e62-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2e62-130">Type</span></span>|<span data-ttu-id="a2e62-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e62-132">id</span><span class="sxs-lookup"><span data-stu-id="a2e62-132">id</span></span>|<span data-ttu-id="a2e62-133">String</span><span class="sxs-lookup"><span data-stu-id="a2e62-133">String</span></span>|<span data-ttu-id="a2e62-134">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="a2e62-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e62-135">createdDateTime</span></span>|<span data-ttu-id="a2e62-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e62-136">DateTimeOffset</span></span>|<span data-ttu-id="a2e62-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a2e62-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="a2e62-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e62-138">lastModifiedDateTime</span></span>|<span data-ttu-id="a2e62-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e62-139">DateTimeOffset</span></span>|<span data-ttu-id="a2e62-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a2e62-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a2e62-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a2e62-141">displayName</span></span>|<span data-ttu-id="a2e62-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2e62-142">String</span></span>|<span data-ttu-id="a2e62-143">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-143">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="a2e62-144">description</span><span class="sxs-lookup"><span data-stu-id="a2e62-144">description</span></span>|<span data-ttu-id="a2e62-145">String</span><span class="sxs-lookup"><span data-stu-id="a2e62-145">String</span></span>|<span data-ttu-id="a2e62-146">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-146">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="a2e62-147">title</span><span class="sxs-lookup"><span data-stu-id="a2e62-147">title</span></span>|<span data-ttu-id="a2e62-148">String</span><span class="sxs-lookup"><span data-stu-id="a2e62-148">String</span></span>|<span data-ttu-id="a2e62-149">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a2e62-149">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="a2e62-150">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-150">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a2e62-151">bodyText</span><span class="sxs-lookup"><span data-stu-id="a2e62-151">bodyText</span></span>|<span data-ttu-id="a2e62-152">String</span><span class="sxs-lookup"><span data-stu-id="a2e62-152">String</span></span>|<span data-ttu-id="a2e62-153">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="a2e62-153">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="a2e62-154">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a2e62-155">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="a2e62-155">acceptanceStatement</span></span>|<span data-ttu-id="a2e62-156">String</span><span class="sxs-lookup"><span data-stu-id="a2e62-156">String</span></span>|<span data-ttu-id="a2e62-157">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-157">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="a2e62-158">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="a2e62-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a2e62-159">version</span><span class="sxs-lookup"><span data-stu-id="a2e62-159">version</span></span>|<span data-ttu-id="a2e62-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e62-160">Int32</span></span>|<span data-ttu-id="a2e62-161">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="a2e62-161">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="a2e62-162">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="a2e62-162">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a2e62-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e62-163">Response</span></span>
<span data-ttu-id="a2e62-164">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e62-164">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e62-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2e62-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2e62-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e62-166">Request</span></span>
<span data-ttu-id="a2e62-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2e62-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="a2e62-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e62-168">Response</span></span>
<span data-ttu-id="a2e62-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2e62-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




