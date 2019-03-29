---
title: Atualizar managementConditionStatement
description: Atualiza as propriedades de um objeto managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c2211d202ddc875a0da24d9f0d5bbe959f092ae
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969404"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="e44ea-103">Atualizar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="e44ea-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="e44ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e44ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e44ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e44ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e44ea-106">Atualiza as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="e44ea-106">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e44ea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e44ea-107">Prerequisites</span></span>
<span data-ttu-id="e44ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e44ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e44ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e44ea-110">Permission type</span></span>|<span data-ttu-id="e44ea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e44ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e44ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e44ea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44ea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e44ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e44ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ea-115">Not supported.</span></span>|
|<span data-ttu-id="e44ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44ea-116">Application</span></span>|<span data-ttu-id="e44ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e44ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="e44ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ea-119">Request headers</span></span>
|<span data-ttu-id="e44ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e44ea-120">Header</span></span>|<span data-ttu-id="e44ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e44ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e44ea-122">Authorization</span></span>|<span data-ttu-id="e44ea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e44ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44ea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e44ea-124">Accept</span></span>|<span data-ttu-id="e44ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e44ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ea-126">Request body</span></span>
<span data-ttu-id="e44ea-127">No corpo da solicitação, forneça uma representação JSON do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="e44ea-127">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="e44ea-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="e44ea-128">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="e44ea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e44ea-129">Property</span></span>|<span data-ttu-id="e44ea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e44ea-130">Type</span></span>|<span data-ttu-id="e44ea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e44ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44ea-132">id</span><span class="sxs-lookup"><span data-stu-id="e44ea-132">id</span></span>|<span data-ttu-id="e44ea-133">String</span><span class="sxs-lookup"><span data-stu-id="e44ea-133">String</span></span>|<span data-ttu-id="e44ea-134">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e44ea-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="e44ea-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="e44ea-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e44ea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e44ea-136">displayName</span></span>|<span data-ttu-id="e44ea-137">String</span><span class="sxs-lookup"><span data-stu-id="e44ea-137">String</span></span>|<span data-ttu-id="e44ea-138">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e44ea-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="e44ea-139">descrição</span><span class="sxs-lookup"><span data-stu-id="e44ea-139">description</span></span>|<span data-ttu-id="e44ea-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e44ea-140">String</span></span>|<span data-ttu-id="e44ea-141">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e44ea-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="e44ea-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e44ea-142">createdDateTime</span></span>|<span data-ttu-id="e44ea-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e44ea-143">DateTimeOffset</span></span>|<span data-ttu-id="e44ea-144">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="e44ea-144">The time the management condition statement was created.</span></span> <span data-ttu-id="e44ea-145">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="e44ea-145">Generated service side.</span></span>|
|<span data-ttu-id="e44ea-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e44ea-146">modifiedDateTime</span></span>|<span data-ttu-id="e44ea-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e44ea-147">DateTimeOffset</span></span>|<span data-ttu-id="e44ea-148">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e44ea-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="e44ea-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="e44ea-149">Updated service side.</span></span>|
|<span data-ttu-id="e44ea-150">expressão</span><span class="sxs-lookup"><span data-stu-id="e44ea-150">expression</span></span>|[<span data-ttu-id="e44ea-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="e44ea-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="e44ea-152">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="e44ea-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="e44ea-153">eTag</span><span class="sxs-lookup"><span data-stu-id="e44ea-153">eTag</span></span>|<span data-ttu-id="e44ea-154">String</span><span class="sxs-lookup"><span data-stu-id="e44ea-154">String</span></span>|<span data-ttu-id="e44ea-155">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e44ea-155">ETag of the management condition statement.</span></span> <span data-ttu-id="e44ea-156">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="e44ea-156">Updated service side.</span></span>|
|<span data-ttu-id="e44ea-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="e44ea-157">applicablePlatforms</span></span>|<span data-ttu-id="e44ea-158">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="e44ea-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e44ea-159">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e44ea-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="e44ea-160">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="e44ea-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="e44ea-161">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="e44ea-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="e44ea-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ea-162">Response</span></span>
<span data-ttu-id="e44ea-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e44ea-163">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e44ea-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e44ea-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e44ea-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ea-165">Request</span></span>
<span data-ttu-id="e44ea-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e44ea-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e44ea-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ea-167">Response</span></span>
<span data-ttu-id="e44ea-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e44ea-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




