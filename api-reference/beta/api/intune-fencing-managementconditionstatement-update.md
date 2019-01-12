---
title: Atualizar managementConditionStatement
description: Atualize as propriedades de um objeto managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 800d40bda342ea23b55e7dc9bf62a99f1e41e3df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935413"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="f21ef-103">Atualizar managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="f21ef-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="f21ef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f21ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f21ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f21ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f21ef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f21ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f21ef-107">Atualize as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="f21ef-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f21ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f21ef-108">Prerequisites</span></span>
<span data-ttu-id="f21ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f21ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f21ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f21ef-111">Permission type</span></span>|<span data-ttu-id="f21ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f21ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f21ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f21ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f21ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f21ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f21ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f21ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f21ef-116">Not supported.</span></span>|
|<span data-ttu-id="f21ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f21ef-117">Application</span></span>|<span data-ttu-id="f21ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f21ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f21ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f21ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="f21ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f21ef-120">Request headers</span></span>
|<span data-ttu-id="f21ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f21ef-121">Header</span></span>|<span data-ttu-id="f21ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f21ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f21ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f21ef-123">Authorization</span></span>|<span data-ttu-id="f21ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f21ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f21ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f21ef-125">Accept</span></span>|<span data-ttu-id="f21ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f21ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f21ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f21ef-127">Request body</span></span>
<span data-ttu-id="f21ef-128">No corpo da solicitação, fornece uma representação JSON para o objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="f21ef-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="f21ef-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="f21ef-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="f21ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f21ef-130">Property</span></span>|<span data-ttu-id="f21ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f21ef-131">Type</span></span>|<span data-ttu-id="f21ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21ef-133">id</span><span class="sxs-lookup"><span data-stu-id="f21ef-133">id</span></span>|<span data-ttu-id="f21ef-134">String</span><span class="sxs-lookup"><span data-stu-id="f21ef-134">String</span></span>|<span data-ttu-id="f21ef-135">Identificador exclusivo para a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="f21ef-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f21ef-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f21ef-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f21ef-137">displayName</span></span>|<span data-ttu-id="f21ef-138">String</span><span class="sxs-lookup"><span data-stu-id="f21ef-138">String</span></span>|<span data-ttu-id="f21ef-139">O nome definido admin da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="f21ef-140">description</span><span class="sxs-lookup"><span data-stu-id="f21ef-140">description</span></span>|<span data-ttu-id="f21ef-141">String</span><span class="sxs-lookup"><span data-stu-id="f21ef-141">String</span></span>|<span data-ttu-id="f21ef-142">O administrador definidos descrição da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="f21ef-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f21ef-143">createdDateTime</span></span>|<span data-ttu-id="f21ef-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21ef-144">DateTimeOffset</span></span>|<span data-ttu-id="f21ef-145">A hora em que a declaração de condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="f21ef-145">The time the management condition statement was created.</span></span> <span data-ttu-id="f21ef-146">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="f21ef-146">Generated service side.</span></span>|
|<span data-ttu-id="f21ef-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f21ef-147">modifiedDateTime</span></span>|<span data-ttu-id="f21ef-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21ef-148">DateTimeOffset</span></span>|<span data-ttu-id="f21ef-149">A hora que da última modificação a declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="f21ef-150">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="f21ef-150">Updated service side.</span></span>|
|<span data-ttu-id="f21ef-151">expressão</span><span class="sxs-lookup"><span data-stu-id="f21ef-151">expression</span></span>|[<span data-ttu-id="f21ef-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="f21ef-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="f21ef-153">A expressão da instrução gerenciamento condição usada para avaliar se um gerenciamento de condição instrução foi ativado/desativado.</span><span class="sxs-lookup"><span data-stu-id="f21ef-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="f21ef-154">eTag</span><span class="sxs-lookup"><span data-stu-id="f21ef-154">eTag</span></span>|<span data-ttu-id="f21ef-155">String</span><span class="sxs-lookup"><span data-stu-id="f21ef-155">String</span></span>|<span data-ttu-id="f21ef-156">ETag da declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-156">ETag of the management condition statement.</span></span> <span data-ttu-id="f21ef-157">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="f21ef-157">Updated service side.</span></span>|
|<span data-ttu-id="f21ef-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f21ef-158">applicablePlatforms</span></span>|<span data-ttu-id="f21ef-159">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f21ef-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f21ef-160">As plataformas aplicáveis para esta declaração de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f21ef-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="f21ef-161">Isso é calculado a partir procurando as condições de gerenciamento associadas ao gerenciamento de condição de instrução e encontrar a interseção de plataformas aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="f21ef-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="f21ef-162">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="f21ef-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="f21ef-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21ef-163">Response</span></span>
<span data-ttu-id="f21ef-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f21ef-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f21ef-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f21ef-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="f21ef-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f21ef-166">Request</span></span>
<span data-ttu-id="f21ef-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f21ef-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
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

### <a name="response"></a><span data-ttu-id="f21ef-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21ef-168">Response</span></span>
<span data-ttu-id="f21ef-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f21ef-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





