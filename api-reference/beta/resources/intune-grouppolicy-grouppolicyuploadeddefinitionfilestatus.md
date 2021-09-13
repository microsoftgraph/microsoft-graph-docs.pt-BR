---
title: groupPolicyUploadedDefinitionFileStatus tipo de número
description: Tipo de status de arquivo de definição carregado da Política de Grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 765300d2af833a2dfaa8e6b42aac47281da01d1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030183"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a>groupPolicyUploadedDefinitionFileStatus tipo de número

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de status de arquivo de definição carregado da Política de Grupo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Status de carregamento inválido do arquivo de definição carregado pela Política de Grupo.|
|uploadInProgress|1|Carregamento de arquivo de definição carregado pela Política de Grupo em andamento.|
|disponível|2|Arquivo de definição carregado da Política de Grupo disponível.|
|atribuído|3|Arquivo de definição carregado da Política de Grupo atribuído à política.|
|removalInProgress|4 |A Política de Grupo carregou a remoção do arquivo de definição em andamento.|
|uploadFailed|5 |Falha no carregamento de arquivo de definição carregado pela Política de Grupo.|
|removalFailed|6 |Falha na remoção do arquivo de definição carregado pela Política de Grupo.|



