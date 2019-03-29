---
title: Criar managementConditionStatement
description: Criar um novo objeto managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e4531f8819be505587a27008f36fb9c06f2d92a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971637"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="0c984-103">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="0c984-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="0c984-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c984-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c984-106">Criar um novo objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="0c984-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c984-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c984-107">Prerequisites</span></span>
<span data-ttu-id="0c984-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c984-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c984-110">Permission type</span></span>|<span data-ttu-id="0c984-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c984-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c984-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c984-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c984-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c984-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c984-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c984-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c984-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c984-115">Not supported.</span></span>|
|<span data-ttu-id="0c984-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c984-116">Application</span></span>|<span data-ttu-id="0c984-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c984-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c984-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c984-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="0c984-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c984-119">Request headers</span></span>
|<span data-ttu-id="0c984-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c984-120">Header</span></span>|<span data-ttu-id="0c984-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c984-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c984-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c984-122">Authorization</span></span>|<span data-ttu-id="0c984-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c984-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c984-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c984-124">Accept</span></span>|<span data-ttu-id="0c984-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c984-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c984-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c984-126">Request body</span></span>
<span data-ttu-id="0c984-127">No corpo da solicitação, forneça uma representação JSON do objeto managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="0c984-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="0c984-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="0c984-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="0c984-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c984-129">Property</span></span>|<span data-ttu-id="0c984-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c984-130">Type</span></span>|<span data-ttu-id="0c984-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c984-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c984-132">id</span><span class="sxs-lookup"><span data-stu-id="0c984-132">id</span></span>|<span data-ttu-id="0c984-133">String</span><span class="sxs-lookup"><span data-stu-id="0c984-133">String</span></span>|<span data-ttu-id="0c984-134">Identificador exclusivo da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c984-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="0c984-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="0c984-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0c984-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c984-136">displayName</span></span>|<span data-ttu-id="0c984-137">String</span><span class="sxs-lookup"><span data-stu-id="0c984-137">String</span></span>|<span data-ttu-id="0c984-138">O nome do administrador definido da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c984-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="0c984-139">descrição</span><span class="sxs-lookup"><span data-stu-id="0c984-139">description</span></span>|<span data-ttu-id="0c984-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c984-140">String</span></span>|<span data-ttu-id="0c984-141">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c984-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="0c984-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c984-142">createdDateTime</span></span>|<span data-ttu-id="0c984-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c984-143">DateTimeOffset</span></span>|<span data-ttu-id="0c984-144">A hora em que a instrução de gerenciamento da condição foi criada.</span><span class="sxs-lookup"><span data-stu-id="0c984-144">The time the management condition statement was created.</span></span> <span data-ttu-id="0c984-145">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="0c984-145">Generated service side.</span></span>|
|<span data-ttu-id="0c984-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c984-146">modifiedDateTime</span></span>|<span data-ttu-id="0c984-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c984-147">DateTimeOffset</span></span>|<span data-ttu-id="0c984-148">A hora em que a declaração de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c984-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="0c984-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0c984-149">Updated service side.</span></span>|
|<span data-ttu-id="0c984-150">expressão</span><span class="sxs-lookup"><span data-stu-id="0c984-150">expression</span></span>|[<span data-ttu-id="0c984-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="0c984-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="0c984-152">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="0c984-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="0c984-153">eTag</span><span class="sxs-lookup"><span data-stu-id="0c984-153">eTag</span></span>|<span data-ttu-id="0c984-154">String</span><span class="sxs-lookup"><span data-stu-id="0c984-154">String</span></span>|<span data-ttu-id="0c984-155">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c984-155">ETag of the management condition statement.</span></span> <span data-ttu-id="0c984-156">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0c984-156">Updated service side.</span></span>|
|<span data-ttu-id="0c984-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0c984-157">applicablePlatforms</span></span>|<span data-ttu-id="0c984-158">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="0c984-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0c984-159">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c984-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="0c984-160">Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="0c984-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="0c984-161">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="0c984-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="0c984-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c984-162">Response</span></span>
<span data-ttu-id="0c984-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c984-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c984-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c984-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c984-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c984-165">Request</span></span>
<span data-ttu-id="0c984-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c984-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c984-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c984-167">Response</span></span>
<span data-ttu-id="0c984-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c984-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




