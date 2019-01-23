---
title: Criar groupPolicyPresentationValueLongDecimal
description: Crie um novo objeto de groupPolicyPresentationValueLongDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 51dacbea1970d042d4fe1fb5b3b2bd42f522b131
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429177"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="cf100-103">Criar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="cf100-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="cf100-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf100-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf100-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf100-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf100-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cf100-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf100-107">Crie um novo objeto de [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="cf100-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf100-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf100-108">Prerequisites</span></span>
<span data-ttu-id="cf100-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf100-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf100-111">Permission type</span></span>|<span data-ttu-id="cf100-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf100-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf100-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf100-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf100-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf100-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf100-116">Not supported.</span></span>|
|<span data-ttu-id="cf100-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf100-117">Application</span></span>|<span data-ttu-id="cf100-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf100-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf100-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="cf100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf100-120">Request headers</span></span>
|<span data-ttu-id="cf100-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf100-121">Header</span></span>|<span data-ttu-id="cf100-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf100-123">Authorization</span></span>|<span data-ttu-id="cf100-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf100-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf100-125">Accept</span></span>|<span data-ttu-id="cf100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf100-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf100-127">Request body</span></span>
<span data-ttu-id="cf100-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="cf100-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="cf100-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="cf100-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="cf100-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf100-130">Property</span></span>|<span data-ttu-id="cf100-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf100-131">Type</span></span>|<span data-ttu-id="cf100-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf100-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf100-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf100-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cf100-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf100-134">DateTimeOffset</span></span>|<span data-ttu-id="cf100-135">A data e hora que da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cf100-135">The date and time the object was last modified.</span></span> <span data-ttu-id="cf100-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cf100-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cf100-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf100-137">createdDateTime</span></span>|<span data-ttu-id="cf100-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf100-138">DateTimeOffset</span></span>|<span data-ttu-id="cf100-139">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cf100-139">The date and time the object was created.</span></span> <span data-ttu-id="cf100-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cf100-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cf100-141">id</span><span class="sxs-lookup"><span data-stu-id="cf100-141">id</span></span>|<span data-ttu-id="cf100-142">String</span><span class="sxs-lookup"><span data-stu-id="cf100-142">String</span></span>|<span data-ttu-id="cf100-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf100-143">Key of the entity.</span></span> <span data-ttu-id="cf100-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cf100-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cf100-145">valor</span><span class="sxs-lookup"><span data-stu-id="cf100-145">value</span></span>|<span data-ttu-id="cf100-146">Int64</span><span class="sxs-lookup"><span data-stu-id="cf100-146">Int64</span></span>|<span data-ttu-id="cf100-147">Um valor long não assinado para a apresentação associado.</span><span class="sxs-lookup"><span data-stu-id="cf100-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="cf100-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf100-148">Response</span></span>
<span data-ttu-id="cf100-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf100-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf100-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf100-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf100-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf100-151">Request</span></span>
<span data-ttu-id="cf100-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf100-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="cf100-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf100-153">Response</span></span>
<span data-ttu-id="cf100-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf100-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




