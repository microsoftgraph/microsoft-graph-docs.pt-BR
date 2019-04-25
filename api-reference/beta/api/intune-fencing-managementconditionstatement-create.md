---
title: Criar managementConditionStatement
description: Criar um novo objeto managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0ac7779942e95200556e7d511e24668751690b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532160"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="a1c9d-103">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a1c9d-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="a1c9d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1c9d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c9d-106">Criar um novo objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="a1c9d-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1c9d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1c9d-107">Prerequisites</span></span>
<span data-ttu-id="a1c9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c9d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1c9d-110">Permission type</span></span>|<span data-ttu-id="a1c9d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1c9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1c9d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1c9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1c9d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c9d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1c9d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1c9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1c9d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-115">Not supported.</span></span>|
|<span data-ttu-id="a1c9d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1c9d-116">Application</span></span>|<span data-ttu-id="a1c9d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1c9d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="a1c9d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c9d-119">Request headers</span></span>
|<span data-ttu-id="a1c9d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1c9d-120">Header</span></span>|<span data-ttu-id="a1c9d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1c9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1c9d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1c9d-122">Authorization</span></span>|<span data-ttu-id="a1c9d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1c9d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1c9d-124">Accept</span></span>|<span data-ttu-id="a1c9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1c9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1c9d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c9d-126">Request body</span></span>
<span data-ttu-id="a1c9d-127">No corpo da solicitação, forneça uma representação JSON do objeto managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="a1c9d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="a1c9d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1c9d-129">Property</span></span>|<span data-ttu-id="a1c9d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c9d-130">Type</span></span>|<span data-ttu-id="a1c9d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1c9d-132">id</span><span class="sxs-lookup"><span data-stu-id="a1c9d-132">id</span></span>|<span data-ttu-id="a1c9d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1c9d-133">String</span></span>|<span data-ttu-id="a1c9d-134">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="a1c9d-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a1c9d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a1c9d-136">displayName</span></span>|<span data-ttu-id="a1c9d-137">String</span><span class="sxs-lookup"><span data-stu-id="a1c9d-137">String</span></span>|<span data-ttu-id="a1c9d-138">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="a1c9d-139">description</span><span class="sxs-lookup"><span data-stu-id="a1c9d-139">description</span></span>|<span data-ttu-id="a1c9d-140">String</span><span class="sxs-lookup"><span data-stu-id="a1c9d-140">String</span></span>|<span data-ttu-id="a1c9d-141">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="a1c9d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1c9d-142">createdDateTime</span></span>|<span data-ttu-id="a1c9d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1c9d-143">DateTimeOffset</span></span>|<span data-ttu-id="a1c9d-144">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-144">The time the management condition statement was created.</span></span> <span data-ttu-id="a1c9d-145">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-145">Generated service side.</span></span>|
|<span data-ttu-id="a1c9d-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1c9d-146">modifiedDateTime</span></span>|<span data-ttu-id="a1c9d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1c9d-147">DateTimeOffset</span></span>|<span data-ttu-id="a1c9d-148">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="a1c9d-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-149">Updated service side.</span></span>|
|<span data-ttu-id="a1c9d-150">expressão</span><span class="sxs-lookup"><span data-stu-id="a1c9d-150">expression</span></span>|[<span data-ttu-id="a1c9d-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="a1c9d-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="a1c9d-152">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="a1c9d-153">eTag</span><span class="sxs-lookup"><span data-stu-id="a1c9d-153">eTag</span></span>|<span data-ttu-id="a1c9d-154">String</span><span class="sxs-lookup"><span data-stu-id="a1c9d-154">String</span></span>|<span data-ttu-id="a1c9d-155">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-155">ETag of the management condition statement.</span></span> <span data-ttu-id="a1c9d-156">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-156">Updated service side.</span></span>|
|<span data-ttu-id="a1c9d-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a1c9d-157">applicablePlatforms</span></span>|<span data-ttu-id="a1c9d-158">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="a1c9d-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a1c9d-159">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="a1c9d-160">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="a1c9d-161">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1c9d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c9d-162">Response</span></span>
<span data-ttu-id="a1c9d-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c9d-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1c9d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1c9d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c9d-165">Request</span></span>
<span data-ttu-id="a1c9d-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
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

### <a name="response"></a><span data-ttu-id="a1c9d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c9d-167">Response</span></span>
<span data-ttu-id="a1c9d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1c9d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





