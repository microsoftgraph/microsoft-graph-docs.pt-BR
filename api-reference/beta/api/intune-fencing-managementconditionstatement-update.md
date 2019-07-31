---
title: Atualizar managementConditionStatement
description: Atualiza as propriedades de um objeto managementConditionStatement.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e7a9a0c6cdbee6aae2afbd131674e3d19a12d39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990271"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="0b8cf-103">Atualizar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="0b8cf-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="0b8cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b8cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b8cf-106">Atualiza as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="0b8cf-106">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b8cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b8cf-107">Prerequisites</span></span>
<span data-ttu-id="0b8cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b8cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b8cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b8cf-110">Permission type</span></span>|<span data-ttu-id="0b8cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b8cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b8cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b8cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b8cf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8cf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b8cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b8cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b8cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-115">Not supported.</span></span>|
|<span data-ttu-id="0b8cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b8cf-116">Application</span></span>|<span data-ttu-id="0b8cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b8cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="0b8cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8cf-119">Request headers</span></span>
|<span data-ttu-id="0b8cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b8cf-120">Header</span></span>|<span data-ttu-id="0b8cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b8cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b8cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b8cf-122">Authorization</span></span>|<span data-ttu-id="0b8cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b8cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b8cf-124">Accept</span></span>|<span data-ttu-id="0b8cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b8cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b8cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8cf-126">Request body</span></span>
<span data-ttu-id="0b8cf-127">No corpo da solicitação, forneça uma representação JSON do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="0b8cf-127">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="0b8cf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="0b8cf-128">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="0b8cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b8cf-129">Property</span></span>|<span data-ttu-id="0b8cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b8cf-130">Type</span></span>|<span data-ttu-id="0b8cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b8cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b8cf-132">id</span><span class="sxs-lookup"><span data-stu-id="0b8cf-132">id</span></span>|<span data-ttu-id="0b8cf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b8cf-133">String</span></span>|<span data-ttu-id="0b8cf-134">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="0b8cf-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0b8cf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0b8cf-136">displayName</span></span>|<span data-ttu-id="0b8cf-137">String</span><span class="sxs-lookup"><span data-stu-id="0b8cf-137">String</span></span>|<span data-ttu-id="0b8cf-138">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="0b8cf-139">descrição</span><span class="sxs-lookup"><span data-stu-id="0b8cf-139">description</span></span>|<span data-ttu-id="0b8cf-140">String</span><span class="sxs-lookup"><span data-stu-id="0b8cf-140">String</span></span>|<span data-ttu-id="0b8cf-141">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="0b8cf-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b8cf-142">createdDateTime</span></span>|<span data-ttu-id="0b8cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b8cf-143">DateTimeOffset</span></span>|<span data-ttu-id="0b8cf-144">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-144">The time the management condition statement was created.</span></span> <span data-ttu-id="0b8cf-145">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-145">Generated service side.</span></span>|
|<span data-ttu-id="0b8cf-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b8cf-146">modifiedDateTime</span></span>|<span data-ttu-id="0b8cf-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b8cf-147">DateTimeOffset</span></span>|<span data-ttu-id="0b8cf-148">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="0b8cf-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-149">Updated service side.</span></span>|
|<span data-ttu-id="0b8cf-150">expressão</span><span class="sxs-lookup"><span data-stu-id="0b8cf-150">expression</span></span>|[<span data-ttu-id="0b8cf-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="0b8cf-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="0b8cf-152">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="0b8cf-153">eTag</span><span class="sxs-lookup"><span data-stu-id="0b8cf-153">eTag</span></span>|<span data-ttu-id="0b8cf-154">String</span><span class="sxs-lookup"><span data-stu-id="0b8cf-154">String</span></span>|<span data-ttu-id="0b8cf-155">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-155">ETag of the management condition statement.</span></span> <span data-ttu-id="0b8cf-156">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-156">Updated service side.</span></span>|
|<span data-ttu-id="0b8cf-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0b8cf-157">applicablePlatforms</span></span>|<span data-ttu-id="0b8cf-158">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="0b8cf-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0b8cf-159">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="0b8cf-160">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="0b8cf-161">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="0b8cf-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8cf-162">Response</span></span>
<span data-ttu-id="0b8cf-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-163">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8cf-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b8cf-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b8cf-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8cf-165">Request</span></span>
<span data-ttu-id="0b8cf-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b8cf-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8cf-167">Response</span></span>
<span data-ttu-id="0b8cf-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b8cf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





