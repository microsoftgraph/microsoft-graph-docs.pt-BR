---
title: Tipo de recurso userInstallStateSummary
description: Contém as propriedades do resumo de estado de instalação de um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 079ec07de60da363f4ebe90e0a1fd039aa7a52c10c4b2916ac440faed0983014
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229238"
---
# <a name="userinstallstatesummary-resource-type"></a>Tipo de recurso userInstallStateSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do resumo de estado de instalação de um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userInstallStateSummaries](../api/intune-books-userinstallstatesummary-list.md)|Conjunto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Listar propriedades e relações de objetos de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Obter userInstallStateSummary](../api/intune-books-userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Ler propriedades e relações de objetos de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Criar userInstallStateSummary](../api/intune-books-userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Criar um novo objeto de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Excluir userInstallStateSummary](../api/intune-books-userinstallstatesummary-delete.md)|Nenhum|Excluir [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Atualizar userInstallStateSummary](../api/intune-books-userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Atualizar as propriedades de um objeto de [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userName|Cadeia de caracteres|Nome de usuário.|
|installedDeviceCount|Int32|Contagem de dispositivos instalados.|
|failedDeviceCount|Int32|Falha na contagem de dispositivos.|
|notInstalledDeviceCount|Int32|Sem contagem de dispositivos instalados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceStates|Conjunto [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|O estado de instalação do livro eletrônico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




