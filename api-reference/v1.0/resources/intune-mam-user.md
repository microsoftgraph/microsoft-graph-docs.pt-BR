---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5f9c0ab08db3c8b9f6e48138e31d091ab5dde9a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755211"
---
# <a name="user-resource-type"></a><span data-ttu-id="292a4-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="292a4-103">user resource type</span></span>

<span data-ttu-id="292a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="292a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="292a4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="292a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="292a4-106">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="292a4-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="292a4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="292a4-107">Methods</span></span>
|<span data-ttu-id="292a4-108">Método</span><span class="sxs-lookup"><span data-stu-id="292a4-108">Method</span></span>|<span data-ttu-id="292a4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="292a4-109">Return Type</span></span>|<span data-ttu-id="292a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="292a4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="292a4-111">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="292a4-111">List users</span></span>](../api/intune-mam-user-list.md)|<span data-ttu-id="292a4-112">Coleção [user](../resources/intune-mam-user.md)</span><span class="sxs-lookup"><span data-stu-id="292a4-112">[user](../resources/intune-mam-user.md) collection</span></span>|<span data-ttu-id="292a4-113">Listar propriedades e relações de objetos de [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="292a4-113">List properties and relationships of the [user](../resources/intune-mam-user.md) objects.</span></span>|
|[<span data-ttu-id="292a4-114">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="292a4-114">Get user</span></span>](../api/intune-mam-user-get.md)|[<span data-ttu-id="292a4-115">user</span><span class="sxs-lookup"><span data-stu-id="292a4-115">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="292a4-116">Ler propriedades e relações de objetos de [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="292a4-116">Read properties and relationships of the [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="292a4-117">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="292a4-117">Create user</span></span>](../api/intune-mam-user-create.md)|[<span data-ttu-id="292a4-118">user</span><span class="sxs-lookup"><span data-stu-id="292a4-118">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="292a4-119">Criar um novo objeto de [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="292a4-119">Create a new [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="292a4-120">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="292a4-120">Delete user</span></span>](../api/intune-mam-user-delete.md)|<span data-ttu-id="292a4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="292a4-121">None</span></span>|<span data-ttu-id="292a4-122">Excluir [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="292a4-122">Deletes a [user](../resources/intune-mam-user.md).</span></span>|
|[<span data-ttu-id="292a4-123">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="292a4-123">Update user</span></span>](../api/intune-mam-user-update.md)|[<span data-ttu-id="292a4-124">user</span><span class="sxs-lookup"><span data-stu-id="292a4-124">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="292a4-125">Atualizar as propriedades de um objeto de [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="292a4-125">Update the properties of a [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="292a4-126">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="292a4-126">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="292a4-127">Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="292a4-127">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="292a4-128">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="292a4-128">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="292a4-129">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="292a4-129">getManagedAppPolicies function</span></span>](../api/intune-mam-user-getmanagedapppolicies.md)|<span data-ttu-id="292a4-130">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="292a4-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="292a4-131">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="292a4-131">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="292a4-132">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="292a4-132">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="292a4-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="292a4-133">None</span></span>|<span data-ttu-id="292a4-134">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="292a4-134">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="292a4-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="292a4-135">Properties</span></span>
|<span data-ttu-id="292a4-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="292a4-136">Property</span></span>|<span data-ttu-id="292a4-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="292a4-137">Type</span></span>|<span data-ttu-id="292a4-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="292a4-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="292a4-139">id</span><span class="sxs-lookup"><span data-stu-id="292a4-139">id</span></span>|<span data-ttu-id="292a4-140">String</span><span class="sxs-lookup"><span data-stu-id="292a4-140">String</span></span>|<span data-ttu-id="292a4-141">O identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="292a4-141">The user identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="292a4-142">Relações</span><span class="sxs-lookup"><span data-stu-id="292a4-142">Relationships</span></span>
|<span data-ttu-id="292a4-143">Relação</span><span class="sxs-lookup"><span data-stu-id="292a4-143">Relationship</span></span>|<span data-ttu-id="292a4-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="292a4-144">Type</span></span>|<span data-ttu-id="292a4-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="292a4-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="292a4-146">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="292a4-146">managedAppRegistrations</span></span>|<span data-ttu-id="292a4-147">Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="292a4-147">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="292a4-148">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="292a4-148">Zero or more managed app registrations that belong to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="292a4-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="292a4-149">JSON Representation</span></span>
<span data-ttu-id="292a4-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="292a4-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




