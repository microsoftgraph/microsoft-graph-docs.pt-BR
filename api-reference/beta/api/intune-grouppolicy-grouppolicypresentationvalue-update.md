---
title: Atualizar groupPolicyPresentationValue
description: Atualize as propriedades de um objeto groupPolicyPresentationValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfec8c5c0a228bf4ba1ed360339d4194cc877faf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429148"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="e2596-103">Atualizar groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="e2596-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="e2596-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2596-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2596-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2596-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2596-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e2596-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2596-107">Atualize as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="e2596-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2596-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2596-108">Prerequisites</span></span>
<span data-ttu-id="e2596-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2596-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e2596-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2596-111">Permission type</span></span>|<span data-ttu-id="e2596-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2596-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2596-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2596-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2596-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2596-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2596-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2596-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2596-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2596-116">Not supported.</span></span>|
|<span data-ttu-id="e2596-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2596-117">Application</span></span>|<span data-ttu-id="e2596-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2596-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2596-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2596-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="e2596-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2596-120">Request headers</span></span>
|<span data-ttu-id="e2596-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2596-121">Header</span></span>|<span data-ttu-id="e2596-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2596-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2596-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2596-123">Authorization</span></span>|<span data-ttu-id="e2596-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2596-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2596-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2596-125">Accept</span></span>|<span data-ttu-id="e2596-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2596-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2596-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2596-127">Request body</span></span>
<span data-ttu-id="e2596-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="e2596-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="e2596-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="e2596-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="e2596-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2596-130">Property</span></span>|<span data-ttu-id="e2596-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2596-131">Type</span></span>|<span data-ttu-id="e2596-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2596-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2596-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2596-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e2596-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2596-134">DateTimeOffset</span></span>|<span data-ttu-id="e2596-135">A data e hora que da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e2596-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="e2596-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2596-136">createdDateTime</span></span>|<span data-ttu-id="e2596-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2596-137">DateTimeOffset</span></span>|<span data-ttu-id="e2596-138">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e2596-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="e2596-139">id</span><span class="sxs-lookup"><span data-stu-id="e2596-139">id</span></span>|<span data-ttu-id="e2596-140">String</span><span class="sxs-lookup"><span data-stu-id="e2596-140">String</span></span>|<span data-ttu-id="e2596-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2596-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e2596-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2596-142">Response</span></span>
<span data-ttu-id="e2596-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2596-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2596-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2596-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2596-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2596-145">Request</span></span>
<span data-ttu-id="e2596-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2596-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="e2596-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2596-147">Response</span></span>
<span data-ttu-id="e2596-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2596-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




