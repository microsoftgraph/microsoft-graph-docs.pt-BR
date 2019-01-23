---
title: Atualizar groupPolicyPresentationValueText
description: Atualize as propriedades de um objeto groupPolicyPresentationValueText.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f0a1222c9abac4cbc459f25444e3cb37d6576a7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429170"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="f4ac4-103">Atualizar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="f4ac4-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="f4ac4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4ac4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4ac4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4ac4-107">Atualize as propriedades de um objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f4ac4-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4ac4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4ac4-108">Prerequisites</span></span>
<span data-ttu-id="f4ac4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4ac4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4ac4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4ac4-111">Permission type</span></span>|<span data-ttu-id="f4ac4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4ac4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4ac4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ac4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4ac4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4ac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-116">Not supported.</span></span>|
|<span data-ttu-id="f4ac4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4ac4-117">Application</span></span>|<span data-ttu-id="f4ac4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4ac4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4ac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f4ac4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ac4-120">Request headers</span></span>
|<span data-ttu-id="f4ac4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4ac4-121">Header</span></span>|<span data-ttu-id="f4ac4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4ac4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4ac4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4ac4-123">Authorization</span></span>|<span data-ttu-id="f4ac4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4ac4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4ac4-125">Accept</span></span>|<span data-ttu-id="f4ac4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4ac4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4ac4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ac4-127">Request body</span></span>
<span data-ttu-id="f4ac4-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f4ac4-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="f4ac4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span><span class="sxs-lookup"><span data-stu-id="f4ac4-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="f4ac4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ac4-130">Property</span></span>|<span data-ttu-id="f4ac4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ac4-131">Type</span></span>|<span data-ttu-id="f4ac4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ac4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4ac4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ac4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f4ac4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ac4-134">DateTimeOffset</span></span>|<span data-ttu-id="f4ac4-135">A data e hora que da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-135">The date and time the object was last modified.</span></span> <span data-ttu-id="f4ac4-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f4ac4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ac4-137">createdDateTime</span></span>|<span data-ttu-id="f4ac4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ac4-138">DateTimeOffset</span></span>|<span data-ttu-id="f4ac4-139">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-139">The date and time the object was created.</span></span> <span data-ttu-id="f4ac4-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f4ac4-141">id</span><span class="sxs-lookup"><span data-stu-id="f4ac4-141">id</span></span>|<span data-ttu-id="f4ac4-142">String</span><span class="sxs-lookup"><span data-stu-id="f4ac4-142">String</span></span>|<span data-ttu-id="f4ac4-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-143">Key of the entity.</span></span> <span data-ttu-id="f4ac4-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f4ac4-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f4ac4-145">valor</span><span class="sxs-lookup"><span data-stu-id="f4ac4-145">value</span></span>|<span data-ttu-id="f4ac4-146">String</span><span class="sxs-lookup"><span data-stu-id="f4ac4-146">String</span></span>|<span data-ttu-id="f4ac4-147">Um valor de cadeia de caracteres para a apresentação associado.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f4ac4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ac4-148">Response</span></span>
<span data-ttu-id="f4ac4-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ac4-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4ac4-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4ac4-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ac4-151">Request</span></span>
<span data-ttu-id="f4ac4-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="f4ac4-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ac4-153">Response</span></span>
<span data-ttu-id="f4ac4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4ac4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




