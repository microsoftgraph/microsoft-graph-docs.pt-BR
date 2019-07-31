---
title: Criar groupPolicyPresentationTextBox
description: Criar um novo objeto groupPolicyPresentationTextBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c7c391d350d9a78cabb410fba81a7d11927e89c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989347"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="a9b36-103">Criar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="a9b36-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="a9b36-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9b36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9b36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b36-106">Criar um novo objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="a9b36-106">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b36-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9b36-107">Prerequisites</span></span>
<span data-ttu-id="a9b36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9b36-110">Permission type</span></span>|<span data-ttu-id="a9b36-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9b36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9b36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b36-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b36-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9b36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9b36-115">Not supported.</span></span>|
|<span data-ttu-id="a9b36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9b36-116">Application</span></span>|<span data-ttu-id="a9b36-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9b36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a9b36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b36-119">Request headers</span></span>
|<span data-ttu-id="a9b36-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9b36-120">Header</span></span>|<span data-ttu-id="a9b36-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a9b36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9b36-122">Authorization</span></span>|<span data-ttu-id="a9b36-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9b36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b36-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9b36-124">Accept</span></span>|<span data-ttu-id="a9b36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b36-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b36-126">Request body</span></span>
<span data-ttu-id="a9b36-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="a9b36-127">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="a9b36-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="a9b36-128">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="a9b36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9b36-129">Property</span></span>|<span data-ttu-id="a9b36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9b36-130">Type</span></span>|<span data-ttu-id="a9b36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9b36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b36-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="a9b36-132">label</span></span>|<span data-ttu-id="a9b36-133">String</span><span class="sxs-lookup"><span data-stu-id="a9b36-133">String</span></span>|<span data-ttu-id="a9b36-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="a9b36-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a9b36-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="a9b36-135">The default value is empty.</span></span> <span data-ttu-id="a9b36-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a9b36-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a9b36-137">id</span><span class="sxs-lookup"><span data-stu-id="a9b36-137">id</span></span>|<span data-ttu-id="a9b36-138">String</span><span class="sxs-lookup"><span data-stu-id="a9b36-138">String</span></span>|<span data-ttu-id="a9b36-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9b36-139">Key of the entity.</span></span> <span data-ttu-id="a9b36-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a9b36-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a9b36-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b36-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a9b36-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b36-142">DateTimeOffset</span></span>|<span data-ttu-id="a9b36-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a9b36-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="a9b36-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a9b36-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a9b36-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a9b36-145">defaultValue</span></span>|<span data-ttu-id="a9b36-146">String</span><span class="sxs-lookup"><span data-stu-id="a9b36-146">String</span></span>|<span data-ttu-id="a9b36-147">Cadeia de caracteres padrão localizada exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="a9b36-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="a9b36-148">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="a9b36-148">The default value is empty.</span></span>|
|<span data-ttu-id="a9b36-149">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a9b36-149">required</span></span>|<span data-ttu-id="a9b36-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9b36-150">Boolean</span></span>|<span data-ttu-id="a9b36-151">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="a9b36-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="a9b36-152">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="a9b36-152">Default value is false.</span></span>|
|<span data-ttu-id="a9b36-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="a9b36-153">maxLength</span></span>|<span data-ttu-id="a9b36-154">Int64</span><span class="sxs-lookup"><span data-stu-id="a9b36-154">Int64</span></span>|<span data-ttu-id="a9b36-155">Um inteiro sem sinal que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="a9b36-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="a9b36-156">O valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="a9b36-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="a9b36-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b36-157">Response</span></span>
<span data-ttu-id="a9b36-158">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b36-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b36-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9b36-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b36-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b36-160">Request</span></span>
<span data-ttu-id="a9b36-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9b36-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="a9b36-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b36-162">Response</span></span>
<span data-ttu-id="a9b36-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9b36-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```





