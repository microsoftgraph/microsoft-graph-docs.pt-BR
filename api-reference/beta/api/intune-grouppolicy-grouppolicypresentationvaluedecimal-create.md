---
title: Criar groupPolicyPresentationValueDecimal
description: Crie um novo objeto de groupPolicyPresentationValueDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32e1947ccbda3b7c7e153daf6058dfc558460a02
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431283"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="61c11-103">Criar groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="61c11-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="61c11-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="61c11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61c11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61c11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61c11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="61c11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61c11-107">Crie um novo objeto de [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="61c11-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61c11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61c11-108">Prerequisites</span></span>
<span data-ttu-id="61c11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="61c11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="61c11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61c11-111">Permission type</span></span>|<span data-ttu-id="61c11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61c11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61c11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61c11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61c11-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c11-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61c11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61c11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61c11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61c11-116">Not supported.</span></span>|
|<span data-ttu-id="61c11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61c11-117">Application</span></span>|<span data-ttu-id="61c11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61c11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61c11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61c11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="61c11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61c11-120">Request headers</span></span>
|<span data-ttu-id="61c11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61c11-121">Header</span></span>|<span data-ttu-id="61c11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61c11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61c11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61c11-123">Authorization</span></span>|<span data-ttu-id="61c11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61c11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61c11-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61c11-125">Accept</span></span>|<span data-ttu-id="61c11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61c11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61c11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61c11-127">Request body</span></span>
<span data-ttu-id="61c11-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="61c11-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="61c11-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="61c11-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="61c11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61c11-130">Property</span></span>|<span data-ttu-id="61c11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61c11-131">Type</span></span>|<span data-ttu-id="61c11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61c11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c11-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61c11-133">lastModifiedDateTime</span></span>|<span data-ttu-id="61c11-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61c11-134">DateTimeOffset</span></span>|<span data-ttu-id="61c11-135">A data e hora que da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="61c11-135">The date and time the object was last modified.</span></span> <span data-ttu-id="61c11-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="61c11-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="61c11-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61c11-137">createdDateTime</span></span>|<span data-ttu-id="61c11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61c11-138">DateTimeOffset</span></span>|<span data-ttu-id="61c11-139">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="61c11-139">The date and time the object was created.</span></span> <span data-ttu-id="61c11-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="61c11-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="61c11-141">id</span><span class="sxs-lookup"><span data-stu-id="61c11-141">id</span></span>|<span data-ttu-id="61c11-142">String</span><span class="sxs-lookup"><span data-stu-id="61c11-142">String</span></span>|<span data-ttu-id="61c11-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61c11-143">Key of the entity.</span></span> <span data-ttu-id="61c11-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="61c11-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="61c11-145">valor</span><span class="sxs-lookup"><span data-stu-id="61c11-145">value</span></span>|<span data-ttu-id="61c11-146">Int64</span><span class="sxs-lookup"><span data-stu-id="61c11-146">Int64</span></span>|<span data-ttu-id="61c11-147">Um valor inteiro não assinado para a apresentação associado.</span><span class="sxs-lookup"><span data-stu-id="61c11-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="61c11-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="61c11-148">Response</span></span>
<span data-ttu-id="61c11-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61c11-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61c11-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61c11-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="61c11-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61c11-151">Request</span></span>
<span data-ttu-id="61c11-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61c11-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="61c11-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="61c11-153">Response</span></span>
<span data-ttu-id="61c11-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61c11-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```




