---
title: Atualizar groupPolicyPresentationValueList
description: Atualize as propriedades de um objeto groupPolicyPresentationValueList.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2eac901bddef0d9063ebd5839031f5b04d009981
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431293"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="0ef99-103">Atualizar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="0ef99-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="0ef99-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ef99-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ef99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ef99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ef99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0ef99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ef99-107">Atualize as propriedades de um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="0ef99-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ef99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ef99-108">Prerequisites</span></span>
<span data-ttu-id="0ef99-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ef99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ef99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ef99-111">Permission type</span></span>|<span data-ttu-id="0ef99-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ef99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ef99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ef99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ef99-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ef99-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ef99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ef99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ef99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ef99-116">Not supported.</span></span>|
|<span data-ttu-id="0ef99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ef99-117">Application</span></span>|<span data-ttu-id="0ef99-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ef99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ef99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ef99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="0ef99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef99-120">Request headers</span></span>
|<span data-ttu-id="0ef99-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ef99-121">Header</span></span>|<span data-ttu-id="0ef99-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ef99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ef99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ef99-123">Authorization</span></span>|<span data-ttu-id="0ef99-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ef99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ef99-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ef99-125">Accept</span></span>|<span data-ttu-id="0ef99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ef99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ef99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef99-127">Request body</span></span>
<span data-ttu-id="0ef99-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="0ef99-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="0ef99-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="0ef99-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="0ef99-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ef99-130">Property</span></span>|<span data-ttu-id="0ef99-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ef99-131">Type</span></span>|<span data-ttu-id="0ef99-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ef99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef99-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef99-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0ef99-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef99-134">DateTimeOffset</span></span>|<span data-ttu-id="0ef99-135">A data e hora que da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0ef99-135">The date and time the object was last modified.</span></span> <span data-ttu-id="0ef99-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0ef99-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0ef99-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef99-137">createdDateTime</span></span>|<span data-ttu-id="0ef99-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef99-138">DateTimeOffset</span></span>|<span data-ttu-id="0ef99-139">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0ef99-139">The date and time the object was created.</span></span> <span data-ttu-id="0ef99-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0ef99-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0ef99-141">id</span><span class="sxs-lookup"><span data-stu-id="0ef99-141">id</span></span>|<span data-ttu-id="0ef99-142">String</span><span class="sxs-lookup"><span data-stu-id="0ef99-142">String</span></span>|<span data-ttu-id="0ef99-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ef99-143">Key of the entity.</span></span> <span data-ttu-id="0ef99-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0ef99-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0ef99-145">values</span><span class="sxs-lookup"><span data-stu-id="0ef99-145">values</span></span>|<span data-ttu-id="0ef99-146">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0ef99-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0ef99-147">Uma lista de pares para a apresentação associado.</span><span class="sxs-lookup"><span data-stu-id="0ef99-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="0ef99-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ef99-148">Response</span></span>
<span data-ttu-id="0ef99-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ef99-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ef99-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ef99-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ef99-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ef99-151">Request</span></span>
<span data-ttu-id="0ef99-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ef99-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0ef99-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ef99-153">Response</span></span>
<span data-ttu-id="0ef99-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ef99-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




