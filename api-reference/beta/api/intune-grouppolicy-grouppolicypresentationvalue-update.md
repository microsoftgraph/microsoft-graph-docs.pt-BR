---
title: Atualizar groupPolicyPresentationValue
description: Atualiza as propriedades de um objeto groupPolicyPresentationValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a5a27308d58c4134e48d86a5fc539c8f16c78f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227445"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="852e0-103">Atualizar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="852e0-103">Update groupPolicyPresentationValue</span></span>

<span data-ttu-id="852e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="852e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="852e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="852e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="852e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="852e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="852e0-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="852e0-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="852e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="852e0-108">Prerequisites</span></span>
<span data-ttu-id="852e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="852e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="852e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="852e0-111">Permission type</span></span>|<span data-ttu-id="852e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="852e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="852e0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="852e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="852e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="852e0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="852e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="852e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="852e0-116">Not supported.</span></span>|
|<span data-ttu-id="852e0-117">Application</span><span class="sxs-lookup"><span data-stu-id="852e0-117">Application</span></span>|<span data-ttu-id="852e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="852e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="852e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="852e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="852e0-120">Request headers</span></span>
|<span data-ttu-id="852e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="852e0-121">Header</span></span>|<span data-ttu-id="852e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="852e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="852e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="852e0-123">Authorization</span></span>|<span data-ttu-id="852e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="852e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="852e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="852e0-125">Accept</span></span>|<span data-ttu-id="852e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="852e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="852e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="852e0-127">Request body</span></span>
<span data-ttu-id="852e0-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="852e0-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="852e0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="852e0-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="852e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="852e0-130">Property</span></span>|<span data-ttu-id="852e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="852e0-131">Type</span></span>|<span data-ttu-id="852e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="852e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="852e0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="852e0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="852e0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="852e0-134">DateTimeOffset</span></span>|<span data-ttu-id="852e0-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="852e0-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="852e0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="852e0-136">createdDateTime</span></span>|<span data-ttu-id="852e0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="852e0-137">DateTimeOffset</span></span>|<span data-ttu-id="852e0-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="852e0-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="852e0-139">id</span><span class="sxs-lookup"><span data-stu-id="852e0-139">id</span></span>|<span data-ttu-id="852e0-140">String</span><span class="sxs-lookup"><span data-stu-id="852e0-140">String</span></span>|<span data-ttu-id="852e0-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="852e0-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="852e0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="852e0-142">Response</span></span>
<span data-ttu-id="852e0-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="852e0-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="852e0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="852e0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="852e0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="852e0-145">Request</span></span>
<span data-ttu-id="852e0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="852e0-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="852e0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="852e0-147">Response</span></span>
<span data-ttu-id="852e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="852e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




