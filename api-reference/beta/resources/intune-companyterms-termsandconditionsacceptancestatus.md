---
title: Tipo de recurso termsAndConditionsAcceptanceStatus
description: Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42bcf4b2b8aaaf82369b0cbf47cd7a6487c06fcd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069352"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a>Tipo de recurso termsAndConditionsAcceptanceStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsAcceptanceStatuses](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Obter termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Criar termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Excluir termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|Nenhuma|Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Atualizar termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário cuja aceitação a entidade representa.|
|acceptedVersion|Int32|Número da versão mais recente dos T&C aceitos pelo usuário.|
|acceptedDateTime|DateTimeOffset|A data e a hora em que os termos foram aceitos pela última vez pelo usuário.|
|userPrincipalName|Cadeia de caracteres|O userPrincipalName do Usuário que aceitou o termo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Link de navegação para os termos e condições atribuídos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



