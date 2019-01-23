---
title: Atualizar deviceConfigurationConflictSummary
description: Atualize as propriedades de um objeto deviceConfigurationConflictSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ad5c5c7ad9db02afed53b4deb0cb6af3d2c57e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416353"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="7f8d1-103">Atualizar deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="7f8d1-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="7f8d1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f8d1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f8d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f8d1-107">Atualize as propriedades de um objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7f8d1-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f8d1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f8d1-108">Prerequisites</span></span>
<span data-ttu-id="7f8d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f8d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f8d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f8d1-111">Permission type</span></span>|<span data-ttu-id="7f8d1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f8d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f8d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f8d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f8d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f8d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f8d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f8d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-116">Not supported.</span></span>|
|<span data-ttu-id="7f8d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f8d1-117">Application</span></span>|<span data-ttu-id="7f8d1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f8d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f8d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7f8d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8d1-120">Request headers</span></span>
|<span data-ttu-id="7f8d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f8d1-121">Header</span></span>|<span data-ttu-id="7f8d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f8d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f8d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f8d1-123">Authorization</span></span>|<span data-ttu-id="7f8d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f8d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f8d1-125">Accept</span></span>|<span data-ttu-id="7f8d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f8d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f8d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8d1-127">Request body</span></span>
<span data-ttu-id="7f8d1-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7f8d1-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="7f8d1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7f8d1-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="7f8d1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f8d1-130">Property</span></span>|<span data-ttu-id="7f8d1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f8d1-131">Type</span></span>|<span data-ttu-id="7f8d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f8d1-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="7f8d1-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="7f8d1-134">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="7f8d1-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7f8d1-135">O conjunto de diretivas em conflito com a configuração de determinado</span><span class="sxs-lookup"><span data-stu-id="7f8d1-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="7f8d1-136">id</span><span class="sxs-lookup"><span data-stu-id="7f8d1-136">id</span></span>|<span data-ttu-id="7f8d1-137">String</span><span class="sxs-lookup"><span data-stu-id="7f8d1-137">String</span></span>|<span data-ttu-id="7f8d1-138">A identificação para este conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="7f8d1-139">Este id é as identificações de todas as políticas do ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="7f8d1-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="7f8d1-140">contributingSettings</span></span>|<span data-ttu-id="7f8d1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="7f8d1-141">String collection</span></span>|<span data-ttu-id="7f8d1-142">O conjunto de configurações em conflito com as políticas de determinado</span><span class="sxs-lookup"><span data-stu-id="7f8d1-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="7f8d1-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="7f8d1-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="7f8d1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7f8d1-144">Int32</span></span>|<span data-ttu-id="7f8d1-145">A contagem de check-ins afetados pelas configurações e diretivas conflitantes</span><span class="sxs-lookup"><span data-stu-id="7f8d1-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="7f8d1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f8d1-146">Response</span></span>
<span data-ttu-id="7f8d1-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f8d1-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f8d1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f8d1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8d1-149">Request</span></span>
<span data-ttu-id="7f8d1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="7f8d1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f8d1-151">Response</span></span>
<span data-ttu-id="7f8d1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f8d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




