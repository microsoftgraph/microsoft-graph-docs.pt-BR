---
title: Tipo de recurso accessPackageResourceAttribute
description: Um recurso que expõe propriedades para o solicitante de um pacote de acesso para fornecer informações personalizadas que podem ser usadas para tomar decisões de aprovação para o pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 27fdb3e5cf90b3a4a7d691b2c44c1d8b36a7d9ab
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468288"
---
# <a name="accesspackageresourceattribute-resource-type"></a>Tipo de recurso accessPackageResourceAttribute

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um atributo de recurso do pacote de acesso é a definição de uma propriedade que um usuário precisa ter para acessar um aplicativo. Essa estrutura está incluída em [um accessPackageResource](../resources/accesspackageresource.md) de um catálogo, para um aplicativo cujas funções são incluídas em um pacote de acesso nesse catálogo. Quando um usuário solicita o pacote de acesso, ele deve fornecer o valor do atributo, que, se a solicitação for aprovada, será gravado no objeto de diretório do usuário. Em seguida, o aplicativo pode [ler o atributo do usuário](../api/user-get.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|Informações sobre como definir o atributo, atualmente um tipo de [objeto accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md) .|
|attributeName|String|O nome do atributo no sistema final. Se o destino for `accessPackageUserDirectoryAttributeStore`, uma propriedade do usuário, como **jobTitle** ou uma extensão de esquema de diretório para o tipo de objeto do usuário, como `extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`. |
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|Informações sobre como preencher o valor do atributo quando um **accessPackageAssignmentRequest** está sendo atendido, atualmente um tipo de objeto [accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md) .|
|id|Cadeia de caracteres|Identificador exclusivo do atributo no recurso do pacote de acesso. Somente leitura. |
|isEditable|Cadeia de caracteres| Especifica se um valor de atributo existente pode ou não ser editado pelo solicitante.|
|isPersistedOnAssignmentRemoval|Boolean| Especifica se o atributo permanecerá no sistema final após o término de uma atribuição.|


### <a name="accesspackageresourceattribute-resource-type-and-extension-properties"></a>AccessPackageResourceAttribute resource type and extension properties

As **propriedades attributeDestination**, **attributeName** e **attributeSource** de um atributo de recurso do pacote de acesso se relacionam às propriedades [de extensão de diretório](extensionproperty.md).

Se **o atributoDestination** for um tipo de objeto [accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md) , o atributo indicado por **attributeName** deve ser uma propriedade writable do [objeto do](user.md) usuário. Essas propriedades writable são tipos de cadeia de caracteres registrados como [propriedades de extensão](extensionproperty.md) no **objeto User de** destino.

Por exemplo, suponha que um aplicativo exija dois atributos de usuário, o cargo de um usuário e seu título pessoal. Os valores desses atributos podem ser sincronizados com o Azure AD a partir dos atributos **local jobTitle** e **personalTitle** do Active Directory. Como **personalTitle** não é uma das propriedades padrão do objeto user [](user.md), isso exigiria a criação de uma extensão de esquema de diretório para adicionar [a](../api/application-post-extensionproperty.md) propriedade **personalTitle** ao tipo de objeto do usuário. Ao criar uma solicitação de recurso para o aplicativo, você pode incluir dois atributos de recurso do pacote de acesso, um para a propriedade **de usuário jobTitle** e outro com o nome da propriedade de extensão de esquema de diretório que foi criada para o título pessoal, `extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`como .

Se o **atributoSource** do atributo for [accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md), o valor fornecido do solicitante será armazenado conforme fornecido no objeto do usuário e disponibilizado para o aplicativo e outros clientes do Microsoft Graph.
## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
  "isPersistedOnAssignmentRemoval": "Boolean"
}
```
