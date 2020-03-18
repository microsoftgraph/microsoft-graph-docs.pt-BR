---
title: Atualizar groupPolicyPresentationValue
description: Atualiza as propriedades de um objeto groupPolicyPresentationValue.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d55b65e6448c51e2ec52698f240b9d12abcf1d06
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804013"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="f7c8b-103">Atualizar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="f7c8b-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="f7c8b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c8b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c8b-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="f7c8b-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7c8b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7c8b-107">Prerequisites</span></span>
<span data-ttu-id="f7c8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c8b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7c8b-110">Permission type</span></span>|<span data-ttu-id="f7c8b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7c8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7c8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7c8b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c8b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7c8b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7c8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-115">Not supported.</span></span>|
|<span data-ttu-id="f7c8b-116">Application</span><span class="sxs-lookup"><span data-stu-id="f7c8b-116">Application</span></span>|<span data-ttu-id="f7c8b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c8b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f7c8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c8b-119">Request headers</span></span>
|<span data-ttu-id="f7c8b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7c8b-120">Header</span></span>|<span data-ttu-id="f7c8b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f7c8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c8b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7c8b-122">Authorization</span></span>|<span data-ttu-id="f7c8b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c8b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7c8b-124">Accept</span></span>|<span data-ttu-id="f7c8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c8b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c8b-126">Request body</span></span>
<span data-ttu-id="f7c8b-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="f7c8b-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="f7c8b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="f7c8b-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="f7c8b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7c8b-129">Property</span></span>|<span data-ttu-id="f7c8b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7c8b-130">Type</span></span>|<span data-ttu-id="f7c8b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7c8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7c8b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7c8b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f7c8b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c8b-133">DateTimeOffset</span></span>|<span data-ttu-id="f7c8b-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="f7c8b-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7c8b-135">createdDateTime</span></span>|<span data-ttu-id="f7c8b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7c8b-136">DateTimeOffset</span></span>|<span data-ttu-id="f7c8b-137">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="f7c8b-138">id</span><span class="sxs-lookup"><span data-stu-id="f7c8b-138">id</span></span>|<span data-ttu-id="f7c8b-139">String</span><span class="sxs-lookup"><span data-stu-id="f7c8b-139">String</span></span>|<span data-ttu-id="f7c8b-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f7c8b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7c8b-141">Response</span></span>
<span data-ttu-id="f7c8b-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c8b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7c8b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c8b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7c8b-144">Request</span></span>
<span data-ttu-id="f7c8b-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="f7c8b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7c8b-146">Response</span></span>
<span data-ttu-id="f7c8b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7c8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




