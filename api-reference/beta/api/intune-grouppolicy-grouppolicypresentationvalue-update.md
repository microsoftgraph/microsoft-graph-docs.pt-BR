---
title: Atualizar groupPolicyPresentationValue
description: Atualiza as propriedades de um objeto groupPolicyPresentationValue.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4796edc39dff60111bef719856f54cf890ae84bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989319"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="335b6-103">Atualizar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="335b6-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="335b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="335b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="335b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="335b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="335b6-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="335b6-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="335b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="335b6-107">Prerequisites</span></span>
<span data-ttu-id="335b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="335b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="335b6-110">Permission type</span></span>|<span data-ttu-id="335b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="335b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="335b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="335b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="335b6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="335b6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="335b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="335b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="335b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="335b6-115">Not supported.</span></span>|
|<span data-ttu-id="335b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="335b6-116">Application</span></span>|<span data-ttu-id="335b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="335b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="335b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="335b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="335b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="335b6-119">Request headers</span></span>
|<span data-ttu-id="335b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="335b6-120">Header</span></span>|<span data-ttu-id="335b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="335b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="335b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="335b6-122">Authorization</span></span>|<span data-ttu-id="335b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="335b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="335b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="335b6-124">Accept</span></span>|<span data-ttu-id="335b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="335b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="335b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="335b6-126">Request body</span></span>
<span data-ttu-id="335b6-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="335b6-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="335b6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="335b6-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="335b6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="335b6-129">Property</span></span>|<span data-ttu-id="335b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="335b6-130">Type</span></span>|<span data-ttu-id="335b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="335b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="335b6-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="335b6-132">lastModifiedDateTime</span></span>|<span data-ttu-id="335b6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="335b6-133">DateTimeOffset</span></span>|<span data-ttu-id="335b6-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="335b6-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="335b6-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="335b6-135">createdDateTime</span></span>|<span data-ttu-id="335b6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="335b6-136">DateTimeOffset</span></span>|<span data-ttu-id="335b6-137">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="335b6-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="335b6-138">id</span><span class="sxs-lookup"><span data-stu-id="335b6-138">id</span></span>|<span data-ttu-id="335b6-139">String</span><span class="sxs-lookup"><span data-stu-id="335b6-139">String</span></span>|<span data-ttu-id="335b6-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="335b6-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="335b6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="335b6-141">Response</span></span>
<span data-ttu-id="335b6-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="335b6-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="335b6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="335b6-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="335b6-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="335b6-144">Request</span></span>
<span data-ttu-id="335b6-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="335b6-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="335b6-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="335b6-146">Response</span></span>
<span data-ttu-id="335b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="335b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





