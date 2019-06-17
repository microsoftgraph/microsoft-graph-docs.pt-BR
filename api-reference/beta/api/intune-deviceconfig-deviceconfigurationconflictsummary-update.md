---
title: Atualizar Propriedadesdeviceconfigurationconflictsummary
description: Atualiza as propriedades de um objeto Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13ee75239a0a50acc6f893cbaa0754318bd79c4e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967787"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="a8fe8-103">Atualizar Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="a8fe8-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="a8fe8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8fe8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8fe8-106">Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a8fe8-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8fe8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8fe8-107">Prerequisites</span></span>
<span data-ttu-id="a8fe8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8fe8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8fe8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8fe8-110">Permission type</span></span>|<span data-ttu-id="a8fe8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8fe8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8fe8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8fe8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8fe8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8fe8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8fe8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8fe8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8fe8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-115">Not supported.</span></span>|
|<span data-ttu-id="a8fe8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8fe8-116">Application</span></span>|<span data-ttu-id="a8fe8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8fe8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8fe8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a8fe8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8fe8-119">Request headers</span></span>
|<span data-ttu-id="a8fe8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8fe8-120">Header</span></span>|<span data-ttu-id="a8fe8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8fe8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8fe8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8fe8-122">Authorization</span></span>|<span data-ttu-id="a8fe8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8fe8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8fe8-124">Accept</span></span>|<span data-ttu-id="a8fe8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8fe8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8fe8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8fe8-126">Request body</span></span>
<span data-ttu-id="a8fe8-127">No corpo da solicitação, forneça uma representação JSON do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a8fe8-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="a8fe8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8fe8-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="a8fe8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8fe8-129">Property</span></span>|<span data-ttu-id="a8fe8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8fe8-130">Type</span></span>|<span data-ttu-id="a8fe8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8fe8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8fe8-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="a8fe8-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="a8fe8-133">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a8fe8-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a8fe8-134">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="a8fe8-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="a8fe8-135">id</span><span class="sxs-lookup"><span data-stu-id="a8fe8-135">id</span></span>|<span data-ttu-id="a8fe8-136">String</span><span class="sxs-lookup"><span data-stu-id="a8fe8-136">String</span></span>|<span data-ttu-id="a8fe8-137">A ID desse conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="a8fe8-138">Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="a8fe8-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="a8fe8-139">contributingSettings</span></span>|<span data-ttu-id="a8fe8-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8fe8-140">String collection</span></span>|<span data-ttu-id="a8fe8-141">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="a8fe8-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="a8fe8-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="a8fe8-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="a8fe8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a8fe8-143">Int32</span></span>|<span data-ttu-id="a8fe8-144">A contagem de check-ins impactados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="a8fe8-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="a8fe8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8fe8-145">Response</span></span>
<span data-ttu-id="a8fe8-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8fe8-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8fe8-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8fe8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8fe8-148">Request</span></span>
<span data-ttu-id="a8fe8-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8fe8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8fe8-150">Response</span></span>
<span data-ttu-id="a8fe8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8fe8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





