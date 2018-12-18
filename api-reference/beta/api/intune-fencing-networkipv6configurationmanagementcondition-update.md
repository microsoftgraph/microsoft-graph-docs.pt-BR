---
title: Atualizar networkIPv6ConfigurationManagementCondition
description: Atualize as propriedades de um objeto networkIPv6ConfigurationManagementCondition.
author: tfitzmac
ms.openlocfilehash: 10014f1ddde4914b97f52e92901266e06ae07c99
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357313"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="84769-103">Atualizar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="84769-103">Update networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="84769-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84769-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84769-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84769-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84769-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84769-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84769-107">Atualize as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="84769-107">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84769-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84769-108">Prerequisites</span></span>
<span data-ttu-id="84769-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84769-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84769-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84769-111">Permission type</span></span>|<span data-ttu-id="84769-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84769-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84769-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84769-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84769-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84769-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84769-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84769-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84769-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84769-116">Not supported.</span></span>|
|<span data-ttu-id="84769-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84769-117">Application</span></span>|<span data-ttu-id="84769-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84769-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84769-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84769-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="84769-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84769-120">Request headers</span></span>
|<span data-ttu-id="84769-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84769-121">Header</span></span>|<span data-ttu-id="84769-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84769-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84769-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84769-123">Authorization</span></span>|<span data-ttu-id="84769-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84769-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84769-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84769-125">Accept</span></span>|<span data-ttu-id="84769-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84769-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84769-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84769-127">Request body</span></span>
<span data-ttu-id="84769-128">No corpo da solicitação, fornece uma representação JSON para o objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="84769-128">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="84769-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="84769-129">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="84769-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84769-130">Property</span></span>|<span data-ttu-id="84769-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84769-131">Type</span></span>|<span data-ttu-id="84769-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84769-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84769-133">id</span><span class="sxs-lookup"><span data-stu-id="84769-133">id</span></span>|<span data-ttu-id="84769-134">String</span><span class="sxs-lookup"><span data-stu-id="84769-134">String</span></span>|<span data-ttu-id="84769-135">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="84769-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="84769-136">System generated value assigned when created.</span></span> <span data-ttu-id="84769-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-138">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="84769-138">uniqueName</span></span>|<span data-ttu-id="84769-139">String</span><span class="sxs-lookup"><span data-stu-id="84769-139">String</span></span>|<span data-ttu-id="84769-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-140">Unique name for the management condition.</span></span> <span data-ttu-id="84769-141">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-141">Used in management condition expressions.</span></span> <span data-ttu-id="84769-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-143">displayName</span><span class="sxs-lookup"><span data-stu-id="84769-143">displayName</span></span>|<span data-ttu-id="84769-144">String</span><span class="sxs-lookup"><span data-stu-id="84769-144">String</span></span>|<span data-ttu-id="84769-145">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="84769-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-147">description</span><span class="sxs-lookup"><span data-stu-id="84769-147">description</span></span>|<span data-ttu-id="84769-148">String</span><span class="sxs-lookup"><span data-stu-id="84769-148">String</span></span>|<span data-ttu-id="84769-149">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="84769-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84769-151">createdDateTime</span></span>|<span data-ttu-id="84769-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84769-152">DateTimeOffset</span></span>|<span data-ttu-id="84769-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="84769-153">The time the management condition was created.</span></span> <span data-ttu-id="84769-154">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="84769-154">Generated service side.</span></span> <span data-ttu-id="84769-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84769-156">modifiedDateTime</span></span>|<span data-ttu-id="84769-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84769-157">DateTimeOffset</span></span>|<span data-ttu-id="84769-158">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-158">The time the management condition was last modified.</span></span> <span data-ttu-id="84769-159">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="84769-159">Updated service side.</span></span> <span data-ttu-id="84769-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-161">eTag</span><span class="sxs-lookup"><span data-stu-id="84769-161">eTag</span></span>|<span data-ttu-id="84769-162">String</span><span class="sxs-lookup"><span data-stu-id="84769-162">String</span></span>|<span data-ttu-id="84769-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-163">ETag of the management condition.</span></span> <span data-ttu-id="84769-164">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="84769-164">Updated service side.</span></span> <span data-ttu-id="84769-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="84769-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="84769-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="84769-166">applicablePlatforms</span></span>|<span data-ttu-id="84769-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="84769-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="84769-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="84769-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="84769-169">Herdada do [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="84769-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="84769-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="84769-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="84769-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="84769-171">ipV6Prefix</span></span>|<span data-ttu-id="84769-172">String</span><span class="sxs-lookup"><span data-stu-id="84769-172">String</span></span>|<span data-ttu-id="84769-173">A sub-rede IPv6 seja conectada.</span><span class="sxs-lookup"><span data-stu-id="84769-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="84769-174">Por exemplo, 2001:db8::/ / 32</span><span class="sxs-lookup"><span data-stu-id="84769-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="84769-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="84769-175">ipV6Gateway</span></span>|<span data-ttu-id="84769-176">String</span><span class="sxs-lookup"><span data-stu-id="84769-176">String</span></span>|<span data-ttu-id="84769-177">O endereço de gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="84769-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="84769-178">Por exemplo 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="84769-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="84769-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="84769-179">ipV6DNSServerList</span></span>|<span data-ttu-id="84769-180">String collection</span><span class="sxs-lookup"><span data-stu-id="84769-180">String collection</span></span>|<span data-ttu-id="84769-181">Um IPv6 os servidores DNS configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="84769-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="84769-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="84769-182">dnsSuffixList</span></span>|<span data-ttu-id="84769-183">String collection</span><span class="sxs-lookup"><span data-stu-id="84769-183">String collection</span></span>|<span data-ttu-id="84769-184">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="84769-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="84769-185">Por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="84769-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="84769-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="84769-186">Response</span></span>
<span data-ttu-id="84769-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84769-187">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84769-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84769-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="84769-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84769-189">Request</span></span>
<span data-ttu-id="84769-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84769-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84769-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="84769-191">Response</span></span>
<span data-ttu-id="84769-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84769-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





