---
title: Criar groupPolicyPresentationValue
description: Crie um novo objeto groupPolicyPresentationValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92826f7e68767f4454f2fd1cba9b353c741cdc0f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157381"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="90ca1-103">Criar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90ca1-103">Create groupPolicyPresentationValue</span></span>

<span data-ttu-id="90ca1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ca1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90ca1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90ca1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ca1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90ca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ca1-107">Crie um novo [objeto groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="90ca1-107">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ca1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90ca1-108">Prerequisites</span></span>
<span data-ttu-id="90ca1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ca1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ca1-111">Permission type</span></span>|<span data-ttu-id="90ca1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ca1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ca1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ca1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90ca1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ca1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90ca1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ca1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ca1-116">Not supported.</span></span>|
|<span data-ttu-id="90ca1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ca1-117">Application</span></span>|<span data-ttu-id="90ca1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ca1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ca1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ca1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="90ca1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca1-120">Request headers</span></span>
|<span data-ttu-id="90ca1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90ca1-121">Header</span></span>|<span data-ttu-id="90ca1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90ca1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ca1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ca1-123">Authorization</span></span>|<span data-ttu-id="90ca1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ca1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ca1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90ca1-125">Accept</span></span>|<span data-ttu-id="90ca1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ca1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ca1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca1-127">Request body</span></span>
<span data-ttu-id="90ca1-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValue.</span><span class="sxs-lookup"><span data-stu-id="90ca1-128">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="90ca1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationValue.</span><span class="sxs-lookup"><span data-stu-id="90ca1-129">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="90ca1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90ca1-130">Property</span></span>|<span data-ttu-id="90ca1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90ca1-131">Type</span></span>|<span data-ttu-id="90ca1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ca1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ca1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ca1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="90ca1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ca1-134">DateTimeOffset</span></span>|<span data-ttu-id="90ca1-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90ca1-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="90ca1-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90ca1-136">createdDateTime</span></span>|<span data-ttu-id="90ca1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ca1-137">DateTimeOffset</span></span>|<span data-ttu-id="90ca1-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="90ca1-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="90ca1-139">id</span><span class="sxs-lookup"><span data-stu-id="90ca1-139">id</span></span>|<span data-ttu-id="90ca1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90ca1-140">String</span></span>|<span data-ttu-id="90ca1-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="90ca1-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="90ca1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca1-142">Response</span></span>
<span data-ttu-id="90ca1-143">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca1-143">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ca1-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90ca1-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ca1-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca1-145">Request</span></span>
<span data-ttu-id="90ca1-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ca1-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="90ca1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca1-147">Response</span></span>
<span data-ttu-id="90ca1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ca1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




