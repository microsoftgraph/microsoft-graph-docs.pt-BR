---
title: Criar groupPolicyPresentationListBox
description: Crie um novo objeto de groupPolicyPresentationListBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d080fe046af88939d4c505f3848d1a7f2b1f67d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429047"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="681f2-103">Criar groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="681f2-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="681f2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="681f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="681f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="681f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="681f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="681f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="681f2-107">Crie um novo objeto de [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="681f2-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="681f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="681f2-108">Prerequisites</span></span>
<span data-ttu-id="681f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="681f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="681f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="681f2-111">Permission type</span></span>|<span data-ttu-id="681f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="681f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="681f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="681f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="681f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="681f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="681f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="681f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="681f2-116">Not supported.</span></span>|
|<span data-ttu-id="681f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="681f2-117">Application</span></span>|<span data-ttu-id="681f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="681f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="681f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="681f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="681f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="681f2-120">Request headers</span></span>
|<span data-ttu-id="681f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="681f2-121">Header</span></span>|<span data-ttu-id="681f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="681f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="681f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="681f2-123">Authorization</span></span>|<span data-ttu-id="681f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="681f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="681f2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="681f2-125">Accept</span></span>|<span data-ttu-id="681f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="681f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="681f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="681f2-127">Request body</span></span>
<span data-ttu-id="681f2-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="681f2-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="681f2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="681f2-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="681f2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="681f2-130">Property</span></span>|<span data-ttu-id="681f2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="681f2-131">Type</span></span>|<span data-ttu-id="681f2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="681f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681f2-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="681f2-133">label</span></span>|<span data-ttu-id="681f2-134">String</span><span class="sxs-lookup"><span data-stu-id="681f2-134">String</span></span>|<span data-ttu-id="681f2-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="681f2-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="681f2-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="681f2-136">The default value is empty.</span></span> <span data-ttu-id="681f2-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="681f2-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="681f2-138">id</span><span class="sxs-lookup"><span data-stu-id="681f2-138">id</span></span>|<span data-ttu-id="681f2-139">String</span><span class="sxs-lookup"><span data-stu-id="681f2-139">String</span></span>|<span data-ttu-id="681f2-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="681f2-140">Key of the entity.</span></span> <span data-ttu-id="681f2-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="681f2-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="681f2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="681f2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="681f2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="681f2-143">DateTimeOffset</span></span>|<span data-ttu-id="681f2-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="681f2-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="681f2-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="681f2-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="681f2-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="681f2-146">explicitValue</span></span>|<span data-ttu-id="681f2-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="681f2-147">Boolean</span></span>|<span data-ttu-id="681f2-148">Se essa opção é especificada true o usuário deve especificar o valor da subchave do registro e o nome da subchave do registro.</span><span class="sxs-lookup"><span data-stu-id="681f2-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="681f2-149">Caixa de listagem mostra duas colunas, um para o nome e outro para os dados.</span><span class="sxs-lookup"><span data-stu-id="681f2-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="681f2-150">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="681f2-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="681f2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="681f2-151">Response</span></span>
<span data-ttu-id="681f2-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="681f2-152">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="681f2-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="681f2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="681f2-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="681f2-154">Request</span></span>
<span data-ttu-id="681f2-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="681f2-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="681f2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="681f2-156">Response</span></span>
<span data-ttu-id="681f2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="681f2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




