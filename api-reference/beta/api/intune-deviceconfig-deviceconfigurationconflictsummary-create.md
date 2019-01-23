---
title: Criar deviceConfigurationConflictSummary
description: Crie um novo objeto de deviceConfigurationConflictSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9488f61819a67f7ab648a6677a30e7422be0539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412076"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="916d2-103">Criar deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="916d2-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="916d2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="916d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="916d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="916d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="916d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="916d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="916d2-107">Crie um novo objeto de [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="916d2-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="916d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="916d2-108">Prerequisites</span></span>
<span data-ttu-id="916d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="916d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="916d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="916d2-111">Permission type</span></span>|<span data-ttu-id="916d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="916d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="916d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="916d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="916d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="916d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="916d2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="916d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="916d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916d2-116">Not supported.</span></span>|
|<span data-ttu-id="916d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="916d2-117">Application</span></span>|<span data-ttu-id="916d2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="916d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="916d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="916d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="916d2-120">Request headers</span></span>
|<span data-ttu-id="916d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="916d2-121">Header</span></span>|<span data-ttu-id="916d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="916d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="916d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="916d2-123">Authorization</span></span>|<span data-ttu-id="916d2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="916d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="916d2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="916d2-125">Accept</span></span>|<span data-ttu-id="916d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="916d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="916d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="916d2-127">Request body</span></span>
<span data-ttu-id="916d2-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="916d2-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="916d2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="916d2-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="916d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="916d2-130">Property</span></span>|<span data-ttu-id="916d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="916d2-131">Type</span></span>|<span data-ttu-id="916d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="916d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="916d2-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="916d2-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="916d2-134">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="916d2-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="916d2-135">O conjunto de diretivas em conflito com a configuração de determinado</span><span class="sxs-lookup"><span data-stu-id="916d2-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="916d2-136">id</span><span class="sxs-lookup"><span data-stu-id="916d2-136">id</span></span>|<span data-ttu-id="916d2-137">String</span><span class="sxs-lookup"><span data-stu-id="916d2-137">String</span></span>|<span data-ttu-id="916d2-138">A identificação para este conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="916d2-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="916d2-139">Este id é as identificações de todas as políticas do ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="916d2-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="916d2-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="916d2-140">contributingSettings</span></span>|<span data-ttu-id="916d2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="916d2-141">String collection</span></span>|<span data-ttu-id="916d2-142">O conjunto de configurações em conflito com as políticas de determinado</span><span class="sxs-lookup"><span data-stu-id="916d2-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="916d2-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="916d2-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="916d2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="916d2-144">Int32</span></span>|<span data-ttu-id="916d2-145">A contagem de check-ins afetados pelas configurações e diretivas conflitantes</span><span class="sxs-lookup"><span data-stu-id="916d2-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="916d2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="916d2-146">Response</span></span>
<span data-ttu-id="916d2-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916d2-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916d2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916d2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="916d2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916d2-149">Request</span></span>
<span data-ttu-id="916d2-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916d2-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
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

### <a name="response"></a><span data-ttu-id="916d2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="916d2-151">Response</span></span>
<span data-ttu-id="916d2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="916d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




