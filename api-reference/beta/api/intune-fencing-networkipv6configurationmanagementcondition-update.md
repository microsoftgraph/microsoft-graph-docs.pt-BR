---
title: Atualizar networkIPv6ConfigurationManagementCondition
description: Atualize as propriedades de um objeto networkIPv6ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19f3dbaeffaaad24c90307908037cc8622b333dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991934"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="f866d-103">Atualizar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f866d-103">Update networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="f866d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f866d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f866d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f866d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f866d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f866d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f866d-107">Atualize as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f866d-107">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f866d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f866d-108">Prerequisites</span></span>
<span data-ttu-id="f866d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f866d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f866d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f866d-111">Permission type</span></span>|<span data-ttu-id="f866d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f866d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f866d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f866d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f866d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f866d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f866d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f866d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f866d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f866d-116">Not supported.</span></span>|
|<span data-ttu-id="f866d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f866d-117">Application</span></span>|<span data-ttu-id="f866d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f866d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f866d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f866d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="f866d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f866d-120">Request headers</span></span>
|<span data-ttu-id="f866d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f866d-121">Header</span></span>|<span data-ttu-id="f866d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f866d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f866d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f866d-123">Authorization</span></span>|<span data-ttu-id="f866d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f866d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f866d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f866d-125">Accept</span></span>|<span data-ttu-id="f866d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f866d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f866d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f866d-127">Request body</span></span>
<span data-ttu-id="f866d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f866d-128">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="f866d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f866d-129">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="f866d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f866d-130">Property</span></span>|<span data-ttu-id="f866d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f866d-131">Type</span></span>|<span data-ttu-id="f866d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f866d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f866d-133">id</span><span class="sxs-lookup"><span data-stu-id="f866d-133">id</span></span>|<span data-ttu-id="f866d-134">String</span><span class="sxs-lookup"><span data-stu-id="f866d-134">String</span></span>|<span data-ttu-id="f866d-135">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="f866d-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f866d-136">System generated value assigned when created.</span></span> <span data-ttu-id="f866d-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-138">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="f866d-138">uniqueName</span></span>|<span data-ttu-id="f866d-139">String</span><span class="sxs-lookup"><span data-stu-id="f866d-139">String</span></span>|<span data-ttu-id="f866d-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-140">Unique name for the management condition.</span></span> <span data-ttu-id="f866d-141">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-141">Used in management condition expressions.</span></span> <span data-ttu-id="f866d-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f866d-143">displayName</span></span>|<span data-ttu-id="f866d-144">String</span><span class="sxs-lookup"><span data-stu-id="f866d-144">String</span></span>|<span data-ttu-id="f866d-145">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="f866d-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-147">description</span><span class="sxs-lookup"><span data-stu-id="f866d-147">description</span></span>|<span data-ttu-id="f866d-148">String</span><span class="sxs-lookup"><span data-stu-id="f866d-148">String</span></span>|<span data-ttu-id="f866d-149">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="f866d-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f866d-151">createdDateTime</span></span>|<span data-ttu-id="f866d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f866d-152">DateTimeOffset</span></span>|<span data-ttu-id="f866d-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="f866d-153">The time the management condition was created.</span></span> <span data-ttu-id="f866d-154">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="f866d-154">Generated service side.</span></span> <span data-ttu-id="f866d-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f866d-156">modifiedDateTime</span></span>|<span data-ttu-id="f866d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f866d-157">DateTimeOffset</span></span>|<span data-ttu-id="f866d-158">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-158">The time the management condition was last modified.</span></span> <span data-ttu-id="f866d-159">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="f866d-159">Updated service side.</span></span> <span data-ttu-id="f866d-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-161">eTag</span><span class="sxs-lookup"><span data-stu-id="f866d-161">eTag</span></span>|<span data-ttu-id="f866d-162">String</span><span class="sxs-lookup"><span data-stu-id="f866d-162">String</span></span>|<span data-ttu-id="f866d-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-163">ETag of the management condition.</span></span> <span data-ttu-id="f866d-164">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="f866d-164">Updated service side.</span></span> <span data-ttu-id="f866d-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f866d-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f866d-166">applicablePlatforms</span></span>|<span data-ttu-id="f866d-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f866d-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f866d-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f866d-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f866d-169">Herdada do [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f866d-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f866d-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="f866d-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="f866d-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="f866d-171">ipV6Prefix</span></span>|<span data-ttu-id="f866d-172">String</span><span class="sxs-lookup"><span data-stu-id="f866d-172">String</span></span>|<span data-ttu-id="f866d-173">A sub-rede IPv6 seja conectada.</span><span class="sxs-lookup"><span data-stu-id="f866d-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="f866d-174">Por exemplo, 2001:db8::/ / 32</span><span class="sxs-lookup"><span data-stu-id="f866d-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="f866d-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="f866d-175">ipV6Gateway</span></span>|<span data-ttu-id="f866d-176">String</span><span class="sxs-lookup"><span data-stu-id="f866d-176">String</span></span>|<span data-ttu-id="f866d-177">O endereço de gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="f866d-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="f866d-178">Por exemplo 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="f866d-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="f866d-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="f866d-179">ipV6DNSServerList</span></span>|<span data-ttu-id="f866d-180">String collection</span><span class="sxs-lookup"><span data-stu-id="f866d-180">String collection</span></span>|<span data-ttu-id="f866d-181">Um IPv6 os servidores DNS configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="f866d-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="f866d-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="f866d-182">dnsSuffixList</span></span>|<span data-ttu-id="f866d-183">String collection</span><span class="sxs-lookup"><span data-stu-id="f866d-183">String collection</span></span>|<span data-ttu-id="f866d-184">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="f866d-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="f866d-185">Por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="f866d-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="f866d-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="f866d-186">Response</span></span>
<span data-ttu-id="f866d-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f866d-187">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f866d-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f866d-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="f866d-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f866d-189">Request</span></span>
<span data-ttu-id="f866d-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f866d-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 401

{
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f866d-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="f866d-191">Response</span></span>
<span data-ttu-id="f866d-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f866d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





