---
title: Criar groupPolicyPresentationText
description: Crie um novo objeto de groupPolicyPresentationText.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c2bbc1f04ce351afe75a66dd8596f0b52a81e31
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429126"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="64502-103">Criar groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="64502-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="64502-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="64502-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64502-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64502-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64502-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="64502-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64502-107">Crie um novo objeto de [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="64502-107">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64502-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64502-108">Prerequisites</span></span>
<span data-ttu-id="64502-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="64502-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64502-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64502-111">Permission type</span></span>|<span data-ttu-id="64502-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64502-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64502-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64502-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64502-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64502-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="64502-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64502-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64502-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64502-116">Not supported.</span></span>|
|<span data-ttu-id="64502-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64502-117">Application</span></span>|<span data-ttu-id="64502-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64502-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64502-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64502-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="64502-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64502-120">Request headers</span></span>
|<span data-ttu-id="64502-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64502-121">Header</span></span>|<span data-ttu-id="64502-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64502-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64502-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64502-123">Authorization</span></span>|<span data-ttu-id="64502-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64502-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64502-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64502-125">Accept</span></span>|<span data-ttu-id="64502-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64502-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64502-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64502-127">Request body</span></span>
<span data-ttu-id="64502-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationText.</span><span class="sxs-lookup"><span data-stu-id="64502-128">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="64502-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationText.</span><span class="sxs-lookup"><span data-stu-id="64502-129">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="64502-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64502-130">Property</span></span>|<span data-ttu-id="64502-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64502-131">Type</span></span>|<span data-ttu-id="64502-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64502-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64502-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="64502-133">label</span></span>|<span data-ttu-id="64502-134">String</span><span class="sxs-lookup"><span data-stu-id="64502-134">String</span></span>|<span data-ttu-id="64502-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="64502-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="64502-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="64502-136">The default value is empty.</span></span> <span data-ttu-id="64502-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="64502-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="64502-138">id</span><span class="sxs-lookup"><span data-stu-id="64502-138">id</span></span>|<span data-ttu-id="64502-139">String</span><span class="sxs-lookup"><span data-stu-id="64502-139">String</span></span>|<span data-ttu-id="64502-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64502-140">Key of the entity.</span></span> <span data-ttu-id="64502-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="64502-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="64502-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64502-142">lastModifiedDateTime</span></span>|<span data-ttu-id="64502-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64502-143">DateTimeOffset</span></span>|<span data-ttu-id="64502-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="64502-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="64502-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="64502-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="64502-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="64502-146">Response</span></span>
<span data-ttu-id="64502-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64502-147">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64502-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64502-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="64502-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64502-149">Request</span></span>
<span data-ttu-id="64502-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64502-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="64502-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="64502-151">Response</span></span>
<span data-ttu-id="64502-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64502-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




