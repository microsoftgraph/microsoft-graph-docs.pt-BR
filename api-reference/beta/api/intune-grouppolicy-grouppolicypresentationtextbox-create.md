---
title: Criar groupPolicyPresentationTextBox
description: Crie um novo objeto de groupPolicyPresentationTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20a34e2288541fe948464b1410398138316943a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429193"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="4475c-103">Criar groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="4475c-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="4475c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4475c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4475c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4475c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4475c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4475c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4475c-107">Crie um novo objeto de [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="4475c-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4475c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4475c-108">Prerequisites</span></span>
<span data-ttu-id="4475c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4475c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4475c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4475c-111">Permission type</span></span>|<span data-ttu-id="4475c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4475c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4475c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4475c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4475c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4475c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4475c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4475c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4475c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4475c-116">Not supported.</span></span>|
|<span data-ttu-id="4475c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4475c-117">Application</span></span>|<span data-ttu-id="4475c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4475c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4475c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4475c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="4475c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4475c-120">Request headers</span></span>
|<span data-ttu-id="4475c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4475c-121">Header</span></span>|<span data-ttu-id="4475c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4475c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4475c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4475c-123">Authorization</span></span>|<span data-ttu-id="4475c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4475c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4475c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4475c-125">Accept</span></span>|<span data-ttu-id="4475c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4475c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4475c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4475c-127">Request body</span></span>
<span data-ttu-id="4475c-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="4475c-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="4475c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="4475c-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="4475c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4475c-130">Property</span></span>|<span data-ttu-id="4475c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4475c-131">Type</span></span>|<span data-ttu-id="4475c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4475c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4475c-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="4475c-133">label</span></span>|<span data-ttu-id="4475c-134">String</span><span class="sxs-lookup"><span data-stu-id="4475c-134">String</span></span>|<span data-ttu-id="4475c-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="4475c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="4475c-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="4475c-136">The default value is empty.</span></span> <span data-ttu-id="4475c-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4475c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4475c-138">id</span><span class="sxs-lookup"><span data-stu-id="4475c-138">id</span></span>|<span data-ttu-id="4475c-139">String</span><span class="sxs-lookup"><span data-stu-id="4475c-139">String</span></span>|<span data-ttu-id="4475c-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4475c-140">Key of the entity.</span></span> <span data-ttu-id="4475c-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4475c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4475c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4475c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="4475c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4475c-143">DateTimeOffset</span></span>|<span data-ttu-id="4475c-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4475c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="4475c-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4475c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4475c-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="4475c-146">defaultValue</span></span>|<span data-ttu-id="4475c-147">String</span><span class="sxs-lookup"><span data-stu-id="4475c-147">String</span></span>|<span data-ttu-id="4475c-148">Cadeia de caracteres localizadas padrão exibida na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="4475c-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="4475c-149">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="4475c-149">The default value is empty.</span></span>|
|<span data-ttu-id="4475c-150">obrigatório</span><span class="sxs-lookup"><span data-stu-id="4475c-150">required</span></span>|<span data-ttu-id="4475c-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4475c-151">Boolean</span></span>|<span data-ttu-id="4475c-152">Requisito para inserir um valor na caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="4475c-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="4475c-153">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="4475c-153">Default value is false.</span></span>|
|<span data-ttu-id="4475c-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="4475c-154">maxLength</span></span>|<span data-ttu-id="4475c-155">Int64</span><span class="sxs-lookup"><span data-stu-id="4475c-155">Int64</span></span>|<span data-ttu-id="4475c-156">Um inteiro não assinado que especifica o número máximo de caracteres de texto.</span><span class="sxs-lookup"><span data-stu-id="4475c-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="4475c-157">Valor padrão é 1023.</span><span class="sxs-lookup"><span data-stu-id="4475c-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="4475c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4475c-158">Response</span></span>
<span data-ttu-id="4475c-159">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4475c-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4475c-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4475c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="4475c-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4475c-161">Request</span></span>
<span data-ttu-id="4475c-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4475c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4475c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="4475c-163">Response</span></span>
<span data-ttu-id="4475c-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4475c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




