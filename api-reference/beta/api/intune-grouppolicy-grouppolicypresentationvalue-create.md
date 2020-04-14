---
title: Criar groupPolicyPresentationValue
description: Criar um novo objeto groupPolicyPresentationValue.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d281f6d7b69eeeed72bc854e5bd1aca6ca35720
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461100"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="2dd9b-103">Criar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="2dd9b-103">Create groupPolicyPresentationValue</span></span>

<span data-ttu-id="2dd9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dd9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dd9b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dd9b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dd9b-107">Criar um novo objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="2dd9b-107">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dd9b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2dd9b-108">Prerequisites</span></span>
<span data-ttu-id="2dd9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dd9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dd9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dd9b-111">Permission type</span></span>|<span data-ttu-id="2dd9b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2dd9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dd9b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dd9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2dd9b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dd9b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2dd9b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dd9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dd9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-116">Not supported.</span></span>|
|<span data-ttu-id="2dd9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dd9b-117">Application</span></span>|<span data-ttu-id="2dd9b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dd9b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dd9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dd9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="2dd9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd9b-120">Request headers</span></span>
|<span data-ttu-id="2dd9b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2dd9b-121">Header</span></span>|<span data-ttu-id="2dd9b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2dd9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dd9b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dd9b-123">Authorization</span></span>|<span data-ttu-id="2dd9b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dd9b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2dd9b-125">Accept</span></span>|<span data-ttu-id="2dd9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2dd9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dd9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd9b-127">Request body</span></span>
<span data-ttu-id="2dd9b-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValue.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-128">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="2dd9b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValue.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-129">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="2dd9b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dd9b-130">Property</span></span>|<span data-ttu-id="2dd9b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dd9b-131">Type</span></span>|<span data-ttu-id="2dd9b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dd9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dd9b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd9b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2dd9b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd9b-134">DateTimeOffset</span></span>|<span data-ttu-id="2dd9b-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="2dd9b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd9b-136">createdDateTime</span></span>|<span data-ttu-id="2dd9b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd9b-137">DateTimeOffset</span></span>|<span data-ttu-id="2dd9b-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="2dd9b-139">id</span><span class="sxs-lookup"><span data-stu-id="2dd9b-139">id</span></span>|<span data-ttu-id="2dd9b-140">String</span><span class="sxs-lookup"><span data-stu-id="2dd9b-140">String</span></span>|<span data-ttu-id="2dd9b-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2dd9b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dd9b-142">Response</span></span>
<span data-ttu-id="2dd9b-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-143">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dd9b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dd9b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dd9b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd9b-145">Request</span></span>
<span data-ttu-id="2dd9b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="2dd9b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dd9b-147">Response</span></span>
<span data-ttu-id="2dd9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2dd9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



