# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo enumerado deviceEnrollmentFailureReason

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Principais categorias de falha para inscrição.

## <a name="members"></a>Membros

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Valor padrão, o motivo da falha é desconhecido.|
|autenticação|1|Falha na autenticação|
|autorização|2|Chamada foi autenticada, mas não autorizada a registrar.|
|accountValidation|3|Falha ao validar a conta para o registro. (Conta bloqueada, registro não habilitado)|
|userValidation|4|Usuário não pôde ser validado. (Usuário não existe, não tem licença)|
|deviceNotSupported|5|Gerenciamento de dispositivos móveis não oferece suporte ao dispositivo.|
|inMaintenance|6|Conta está em manutenção.|
|badRequest|7|Cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8|Os recursos usados por esta inscrição não são suportados para essa conta.|
|enrollmentRestrictionsEnforced|9|Restrições de inscrição configuradas pelo administrador bloquearam essa inscrição.|
|clientDisconnected|10|Tempo esgotado ou a inscrição foi anulada pelo usuário final.|
|userAbandonment|11|O registro foi abandonado pelo usuário final. (Usuário iniciou a integração mas não conseguiu concluir a tempo)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->


