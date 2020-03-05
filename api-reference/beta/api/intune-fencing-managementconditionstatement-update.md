---
title: Atualizar managementConditionStatement
description: Atualiza as propriedades de um objeto managementConditionStatement.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7030fe6fcc821e8c20f3ec4c27809217322e7b0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465699"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="0f2c7-103">Atualizar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="0f2c7-103">Update managementConditionStatement</span></span>

<span data-ttu-id="0f2c7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0f2c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f2c7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f2c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f2c7-107">Atualiza as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="0f2c7-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f2c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f2c7-108">Prerequisites</span></span>
<span data-ttu-id="0f2c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f2c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f2c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f2c7-111">Permission type</span></span>|<span data-ttu-id="0f2c7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f2c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f2c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f2c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f2c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f2c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f2c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f2c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f2c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-116">Not supported.</span></span>|
|<span data-ttu-id="0f2c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f2c7-117">Application</span></span>|<span data-ttu-id="0f2c7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f2c7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f2c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f2c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="0f2c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c7-120">Request headers</span></span>
|<span data-ttu-id="0f2c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f2c7-121">Header</span></span>|<span data-ttu-id="0f2c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f2c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f2c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f2c7-123">Authorization</span></span>|<span data-ttu-id="0f2c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f2c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f2c7-125">Accept</span></span>|<span data-ttu-id="0f2c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f2c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f2c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c7-127">Request body</span></span>
<span data-ttu-id="0f2c7-128">No corpo da solicitação, forneça uma representação JSON do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="0f2c7-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="0f2c7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="0f2c7-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="0f2c7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f2c7-130">Property</span></span>|<span data-ttu-id="0f2c7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f2c7-131">Type</span></span>|<span data-ttu-id="0f2c7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f2c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f2c7-133">id</span><span class="sxs-lookup"><span data-stu-id="0f2c7-133">id</span></span>|<span data-ttu-id="0f2c7-134">String</span><span class="sxs-lookup"><span data-stu-id="0f2c7-134">String</span></span>|<span data-ttu-id="0f2c7-135">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="0f2c7-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0f2c7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0f2c7-137">displayName</span></span>|<span data-ttu-id="0f2c7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f2c7-138">String</span></span>|<span data-ttu-id="0f2c7-139">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="0f2c7-140">description</span><span class="sxs-lookup"><span data-stu-id="0f2c7-140">description</span></span>|<span data-ttu-id="0f2c7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f2c7-141">String</span></span>|<span data-ttu-id="0f2c7-142">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="0f2c7-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f2c7-143">createdDateTime</span></span>|<span data-ttu-id="0f2c7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f2c7-144">DateTimeOffset</span></span>|<span data-ttu-id="0f2c7-145">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-145">The time the management condition statement was created.</span></span> <span data-ttu-id="0f2c7-146">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-146">Generated service side.</span></span>|
|<span data-ttu-id="0f2c7-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f2c7-147">modifiedDateTime</span></span>|<span data-ttu-id="0f2c7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f2c7-148">DateTimeOffset</span></span>|<span data-ttu-id="0f2c7-149">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="0f2c7-150">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-150">Updated service side.</span></span>|
|<span data-ttu-id="0f2c7-151">expressão</span><span class="sxs-lookup"><span data-stu-id="0f2c7-151">expression</span></span>|[<span data-ttu-id="0f2c7-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="0f2c7-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="0f2c7-153">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="0f2c7-154">eTag</span><span class="sxs-lookup"><span data-stu-id="0f2c7-154">eTag</span></span>|<span data-ttu-id="0f2c7-155">String</span><span class="sxs-lookup"><span data-stu-id="0f2c7-155">String</span></span>|<span data-ttu-id="0f2c7-156">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-156">ETag of the management condition statement.</span></span> <span data-ttu-id="0f2c7-157">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-157">Updated service side.</span></span>|
|<span data-ttu-id="0f2c7-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0f2c7-158">applicablePlatforms</span></span>|<span data-ttu-id="0f2c7-159">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="0f2c7-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0f2c7-160">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="0f2c7-161">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="0f2c7-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="0f2c7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f2c7-163">Response</span></span>
<span data-ttu-id="0f2c7-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f2c7-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f2c7-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f2c7-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c7-166">Request</span></span>
<span data-ttu-id="0f2c7-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0f2c7-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f2c7-168">Response</span></span>
<span data-ttu-id="0f2c7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f2c7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```





