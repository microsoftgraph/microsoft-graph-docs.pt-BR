---
title: Criar managementConditionStatement
description: Crie um novo objeto de managementConditionStatement.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eba9d3f96d7d3a8b1f855c94b18aab6a6450651f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417354"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="46bac-103">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="46bac-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="46bac-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="46bac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46bac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46bac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46bac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="46bac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46bac-107">Crie um novo objeto de [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="46bac-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46bac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46bac-108">Prerequisites</span></span>
<span data-ttu-id="46bac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="46bac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46bac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46bac-111">Permission type</span></span>|<span data-ttu-id="46bac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46bac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46bac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46bac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46bac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46bac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46bac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46bac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46bac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46bac-116">Not supported.</span></span>|
|<span data-ttu-id="46bac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46bac-117">Application</span></span>|<span data-ttu-id="46bac-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46bac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46bac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46bac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="46bac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46bac-120">Request headers</span></span>
|<span data-ttu-id="46bac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46bac-121">Header</span></span>|<span data-ttu-id="46bac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="46bac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46bac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46bac-123">Authorization</span></span>|<span data-ttu-id="46bac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46bac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46bac-125">Accept</span></span>|<span data-ttu-id="46bac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46bac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46bac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46bac-127">Request body</span></span>
<span data-ttu-id="46bac-128">No corpo da solicitação, fornece uma representação JSON para o objeto managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="46bac-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="46bac-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="46bac-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="46bac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46bac-130">Property</span></span>|<span data-ttu-id="46bac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bac-131">Type</span></span>|<span data-ttu-id="46bac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46bac-133">id</span><span class="sxs-lookup"><span data-stu-id="46bac-133">id</span></span>|<span data-ttu-id="46bac-134">String</span><span class="sxs-lookup"><span data-stu-id="46bac-134">String</span></span>|<span data-ttu-id="46bac-135">Identificador exclusivo para a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="46bac-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="46bac-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="46bac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="46bac-137">displayName</span></span>|<span data-ttu-id="46bac-138">String</span><span class="sxs-lookup"><span data-stu-id="46bac-138">String</span></span>|<span data-ttu-id="46bac-139">O nome definido admin da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="46bac-140">description</span><span class="sxs-lookup"><span data-stu-id="46bac-140">description</span></span>|<span data-ttu-id="46bac-141">String</span><span class="sxs-lookup"><span data-stu-id="46bac-141">String</span></span>|<span data-ttu-id="46bac-142">O administrador definidos descrição da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="46bac-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46bac-143">createdDateTime</span></span>|<span data-ttu-id="46bac-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46bac-144">DateTimeOffset</span></span>|<span data-ttu-id="46bac-145">A hora em que a declaração de condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="46bac-145">The time the management condition statement was created.</span></span> <span data-ttu-id="46bac-146">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="46bac-146">Generated service side.</span></span>|
|<span data-ttu-id="46bac-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46bac-147">modifiedDateTime</span></span>|<span data-ttu-id="46bac-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46bac-148">DateTimeOffset</span></span>|<span data-ttu-id="46bac-149">A hora que da última modificação a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="46bac-150">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="46bac-150">Updated service side.</span></span>|
|<span data-ttu-id="46bac-151">expressão</span><span class="sxs-lookup"><span data-stu-id="46bac-151">expression</span></span>|[<span data-ttu-id="46bac-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="46bac-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="46bac-153">A expressão da instrução gerenciamento condição usada para avaliar se um gerenciamento de condição instrução foi ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="46bac-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="46bac-154">eTag</span><span class="sxs-lookup"><span data-stu-id="46bac-154">eTag</span></span>|<span data-ttu-id="46bac-155">String</span><span class="sxs-lookup"><span data-stu-id="46bac-155">String</span></span>|<span data-ttu-id="46bac-156">ETag da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-156">ETag of the management condition statement.</span></span> <span data-ttu-id="46bac-157">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="46bac-157">Updated service side.</span></span>|
|<span data-ttu-id="46bac-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="46bac-158">applicablePlatforms</span></span>|<span data-ttu-id="46bac-159">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="46bac-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="46bac-160">As plataformas aplicáveis para esta declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46bac-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="46bac-161">Isso é calculado a partir procurando as condições de gerenciamento associadas ao gerenciamento de condição de instrução e encontrar a interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="46bac-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="46bac-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="46bac-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="46bac-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bac-163">Response</span></span>
<span data-ttu-id="46bac-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46bac-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46bac-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46bac-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="46bac-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46bac-166">Request</span></span>
<span data-ttu-id="46bac-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46bac-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46bac-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bac-168">Response</span></span>
<span data-ttu-id="46bac-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46bac-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




