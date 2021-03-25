---
title: Criar managementConditionStatement
description: Crie um novo objeto managementConditionStatement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ad9f8f88d41642dea3090cc05eb8f07f10a10aa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153689"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="a82af-103">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a82af-103">Create managementConditionStatement</span></span>

<span data-ttu-id="a82af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a82af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a82af-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a82af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a82af-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a82af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a82af-107">Crie um novo [objeto managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="a82af-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a82af-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a82af-108">Prerequisites</span></span>
<span data-ttu-id="a82af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a82af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a82af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a82af-111">Permission type</span></span>|<span data-ttu-id="a82af-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a82af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a82af-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a82af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a82af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a82af-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a82af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a82af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82af-116">Not supported.</span></span>|
|<span data-ttu-id="a82af-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a82af-117">Application</span></span>|<span data-ttu-id="a82af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a82af-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a82af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="a82af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a82af-120">Request headers</span></span>
|<span data-ttu-id="a82af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a82af-121">Header</span></span>|<span data-ttu-id="a82af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a82af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a82af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a82af-123">Authorization</span></span>|<span data-ttu-id="a82af-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a82af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a82af-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a82af-125">Accept</span></span>|<span data-ttu-id="a82af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a82af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a82af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a82af-127">Request body</span></span>
<span data-ttu-id="a82af-128">No corpo da solicitação, fornece uma representação JSON para o objeto managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="a82af-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="a82af-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="a82af-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="a82af-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a82af-130">Property</span></span>|<span data-ttu-id="a82af-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a82af-131">Type</span></span>|<span data-ttu-id="a82af-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82af-133">id</span><span class="sxs-lookup"><span data-stu-id="a82af-133">id</span></span>|<span data-ttu-id="a82af-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a82af-134">String</span></span>|<span data-ttu-id="a82af-135">Identificador exclusivo para a instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a82af-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="a82af-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="a82af-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a82af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a82af-137">displayName</span></span>|<span data-ttu-id="a82af-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a82af-138">String</span></span>|<span data-ttu-id="a82af-139">O nome definido pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a82af-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="a82af-140">descrição</span><span class="sxs-lookup"><span data-stu-id="a82af-140">description</span></span>|<span data-ttu-id="a82af-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a82af-141">String</span></span>|<span data-ttu-id="a82af-142">A descrição definida pelo administrador da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a82af-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="a82af-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a82af-143">createdDateTime</span></span>|<span data-ttu-id="a82af-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a82af-144">DateTimeOffset</span></span>|<span data-ttu-id="a82af-145">A hora em que a instrução de condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="a82af-145">The time the management condition statement was created.</span></span> <span data-ttu-id="a82af-146">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="a82af-146">Generated service side.</span></span>|
|<span data-ttu-id="a82af-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a82af-147">modifiedDateTime</span></span>|<span data-ttu-id="a82af-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a82af-148">DateTimeOffset</span></span>|<span data-ttu-id="a82af-149">A hora em que a instrução de condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a82af-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="a82af-150">Lado do serviço atualizado.</span><span class="sxs-lookup"><span data-stu-id="a82af-150">Updated service side.</span></span>|
|<span data-ttu-id="a82af-151">expressão</span><span class="sxs-lookup"><span data-stu-id="a82af-151">expression</span></span>|[<span data-ttu-id="a82af-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="a82af-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="a82af-153">A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.</span><span class="sxs-lookup"><span data-stu-id="a82af-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="a82af-154">eTag</span><span class="sxs-lookup"><span data-stu-id="a82af-154">eTag</span></span>|<span data-ttu-id="a82af-155">String</span><span class="sxs-lookup"><span data-stu-id="a82af-155">String</span></span>|<span data-ttu-id="a82af-156">ETag da instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a82af-156">ETag of the management condition statement.</span></span> <span data-ttu-id="a82af-157">Lado do serviço atualizado.</span><span class="sxs-lookup"><span data-stu-id="a82af-157">Updated service side.</span></span>|
|<span data-ttu-id="a82af-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a82af-158">applicablePlatforms</span></span>|<span data-ttu-id="a82af-159">[Coleção devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="a82af-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a82af-160">As plataformas aplicáveis para essa instrução de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a82af-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="a82af-161">Isso é calculado analisando as condições de gerenciamento associadas à instrução de condição de gerenciamento e encontrando a interseção das plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a82af-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="a82af-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a82af-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="a82af-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82af-163">Response</span></span>
<span data-ttu-id="a82af-164">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a82af-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a82af-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a82af-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="a82af-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a82af-166">Request</span></span>
<span data-ttu-id="a82af-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a82af-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a82af-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82af-168">Response</span></span>
<span data-ttu-id="a82af-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a82af-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 526

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




