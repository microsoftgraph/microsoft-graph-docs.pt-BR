---
title: Criar managementConditionStatement
description: Crie um novo objeto de managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da085e2aa384e2ee3d4eedd611cfe14945b8fe1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806437"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="1ca72-103">Criar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="1ca72-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="1ca72-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ca72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ca72-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ca72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ca72-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ca72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ca72-107">Crie um novo objeto de [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1ca72-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ca72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ca72-108">Prerequisites</span></span>
<span data-ttu-id="1ca72-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ca72-111">Permission type</span></span>|<span data-ttu-id="1ca72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ca72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ca72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ca72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ca72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ca72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ca72-116">Not supported.</span></span>|
|<span data-ttu-id="1ca72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ca72-117">Application</span></span>|<span data-ttu-id="1ca72-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ca72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ca72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ca72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="1ca72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca72-120">Request headers</span></span>
|<span data-ttu-id="1ca72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ca72-121">Header</span></span>|<span data-ttu-id="1ca72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ca72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ca72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ca72-123">Authorization</span></span>|<span data-ttu-id="1ca72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ca72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ca72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ca72-125">Accept</span></span>|<span data-ttu-id="1ca72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ca72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca72-127">Request body</span></span>
<span data-ttu-id="1ca72-128">No corpo da solicitação, fornece uma representação JSON para o objeto managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="1ca72-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="1ca72-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="1ca72-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="1ca72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ca72-130">Property</span></span>|<span data-ttu-id="1ca72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ca72-131">Type</span></span>|<span data-ttu-id="1ca72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ca72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca72-133">id</span><span class="sxs-lookup"><span data-stu-id="1ca72-133">id</span></span>|<span data-ttu-id="1ca72-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ca72-134">String</span></span>|<span data-ttu-id="1ca72-135">Identificador exclusivo para a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="1ca72-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="1ca72-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1ca72-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ca72-137">displayName</span></span>|<span data-ttu-id="1ca72-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ca72-138">String</span></span>|<span data-ttu-id="1ca72-139">O nome definido admin da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="1ca72-140">description</span><span class="sxs-lookup"><span data-stu-id="1ca72-140">description</span></span>|<span data-ttu-id="1ca72-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ca72-141">String</span></span>|<span data-ttu-id="1ca72-142">O administrador definidos descrição da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="1ca72-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca72-143">createdDateTime</span></span>|<span data-ttu-id="1ca72-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ca72-144">DateTimeOffset</span></span>|<span data-ttu-id="1ca72-145">A hora em que a declaração de condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="1ca72-145">The time the management condition statement was created.</span></span> <span data-ttu-id="1ca72-146">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="1ca72-146">Generated service side.</span></span>|
|<span data-ttu-id="1ca72-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca72-147">modifiedDateTime</span></span>|<span data-ttu-id="1ca72-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ca72-148">DateTimeOffset</span></span>|<span data-ttu-id="1ca72-149">A hora que da última modificação a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="1ca72-150">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="1ca72-150">Updated service side.</span></span>|
|<span data-ttu-id="1ca72-151">expressão</span><span class="sxs-lookup"><span data-stu-id="1ca72-151">expression</span></span>|[<span data-ttu-id="1ca72-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="1ca72-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="1ca72-153">A expressão da instrução gerenciamento condição usada para avaliar se um gerenciamento de condição instrução foi ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="1ca72-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="1ca72-154">eTag</span><span class="sxs-lookup"><span data-stu-id="1ca72-154">eTag</span></span>|<span data-ttu-id="1ca72-155">String</span><span class="sxs-lookup"><span data-stu-id="1ca72-155">String</span></span>|<span data-ttu-id="1ca72-156">ETag da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-156">ETag of the management condition statement.</span></span> <span data-ttu-id="1ca72-157">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="1ca72-157">Updated service side.</span></span>|
|<span data-ttu-id="1ca72-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1ca72-158">applicablePlatforms</span></span>|<span data-ttu-id="1ca72-159">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1ca72-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1ca72-160">As plataformas aplicáveis para esta declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1ca72-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="1ca72-161">Isso é calculado a partir procurando as condições de gerenciamento associadas ao gerenciamento de condição de instrução e encontrar a interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="1ca72-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="1ca72-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="1ca72-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ca72-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ca72-163">Response</span></span>
<span data-ttu-id="1ca72-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ca72-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ca72-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ca72-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ca72-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca72-166">Request</span></span>
<span data-ttu-id="1ca72-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ca72-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ca72-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ca72-168">Response</span></span>
<span data-ttu-id="1ca72-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ca72-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





