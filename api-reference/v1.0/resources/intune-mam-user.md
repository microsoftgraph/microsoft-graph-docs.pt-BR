---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88a3b9054e9e274b1acdd4109c6d1b267784cc26
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733707"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um objeto de usuário do Azure Active Directory.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune-mam-user-list.md)|Coleção [user](../resources/intune-mam-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-mam-user.md).|
|[Obter usuário](../api/intune-mam-user-get.md)|[user](../resources/intune-mam-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-mam-user.md).|
|[Criar usuário](../api/intune-mam-user-create.md)|[user](../resources/intune-mam-user.md)|Criar um novo objeto de [user](../resources/intune-mam-user.md).|
|[Excluir usuário](../api/intune-mam-user-delete.md)|Nenhum|Excluir [user](../resources/intune-mam-user.md).|
|[Atualizar usuário](../api/intune-mam-user-update.md)|[user](../resources/intune-mam-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-mam-user.md).|
|[função getManagedAppDiagnosticStatuses](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Obtém diagnóstico do status de validação para um determinado usuário.|
|[Função getManagedAppPolicies](../api/intune-mam-user-getmanagedapppolicies.md)|Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Obtém as restrições de aplicativo para um determinado usuário.|
|[Ação wipeManagedAppRegistrationsByDeviceTag](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|Nenhum|Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedAppRegistrations|Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
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





