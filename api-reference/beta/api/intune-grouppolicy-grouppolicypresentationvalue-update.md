---
title: Atualizar groupPolicyPresentationValue
description: Atualiza as propriedades de um objeto groupPolicyPresentationValue.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b2506663a9cdd79f3ea023c0f969b5a4211acb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464411"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="914a7-103">Atualizar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="914a7-103">Update groupPolicyPresentationValue</span></span>

<span data-ttu-id="914a7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="914a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="914a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="914a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="914a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="914a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914a7-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="914a7-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="914a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="914a7-108">Prerequisites</span></span>
<span data-ttu-id="914a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="914a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="914a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="914a7-111">Permission type</span></span>|<span data-ttu-id="914a7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="914a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="914a7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="914a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="914a7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914a7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="914a7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="914a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="914a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="914a7-116">Not supported.</span></span>|
|<span data-ttu-id="914a7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="914a7-117">Application</span></span>|<span data-ttu-id="914a7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914a7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="914a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="914a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="914a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="914a7-120">Request headers</span></span>
|<span data-ttu-id="914a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="914a7-121">Header</span></span>|<span data-ttu-id="914a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="914a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="914a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="914a7-123">Authorization</span></span>|<span data-ttu-id="914a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="914a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="914a7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="914a7-125">Accept</span></span>|<span data-ttu-id="914a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="914a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="914a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="914a7-127">Request body</span></span>
<span data-ttu-id="914a7-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="914a7-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="914a7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="914a7-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="914a7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="914a7-130">Property</span></span>|<span data-ttu-id="914a7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="914a7-131">Type</span></span>|<span data-ttu-id="914a7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="914a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914a7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="914a7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="914a7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914a7-134">DateTimeOffset</span></span>|<span data-ttu-id="914a7-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="914a7-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="914a7-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="914a7-136">createdDateTime</span></span>|<span data-ttu-id="914a7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914a7-137">DateTimeOffset</span></span>|<span data-ttu-id="914a7-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="914a7-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="914a7-139">id</span><span class="sxs-lookup"><span data-stu-id="914a7-139">id</span></span>|<span data-ttu-id="914a7-140">String</span><span class="sxs-lookup"><span data-stu-id="914a7-140">String</span></span>|<span data-ttu-id="914a7-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="914a7-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="914a7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="914a7-142">Response</span></span>
<span data-ttu-id="914a7-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="914a7-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="914a7-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="914a7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="914a7-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="914a7-145">Request</span></span>
<span data-ttu-id="914a7-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="914a7-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="914a7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="914a7-147">Response</span></span>
<span data-ttu-id="914a7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="914a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





